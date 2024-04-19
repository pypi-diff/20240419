# Comparing `tmp/idinn-0.1.2.tar.gz` & `tmp/idinn-0.1.3.tar.gz`

## Comparing `idinn-0.1.2.tar` & `idinn-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 idinn-0.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 idinn-0.1.2/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/Makefile
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/conf.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/make.bat
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/requirements.txt
--rw-r--r--   0        0        0   453134 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/_static/optimization_schematic.png
--rw-r--r--   0        0        0   243113 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/_static/youtube.png
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/get_started/get_started.rst
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/get_started/installation.rst
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/joss/paper.bib
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/joss/paper.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/tutorials/benchmark.rst
--rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/tutorials/dual.rst
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/tutorials/single.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/tutorials/transfer.rst
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/understand/api.rst
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/understand/dynamics.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/understand/optimization.rst
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/understand/order.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 idinn-0.1.2/docs/understand/straight.rst
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 idinn-0.1.2/src/idinn/__init__.py
--rw-r--r--   0        0        0    32652 2020-02-02 00:00:00.000000 idinn-0.1.2/src/idinn/controller.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 idinn-0.1.2/src/idinn/sourcing_model.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 idinn-0.1.2/tests/test_controller.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 idinn-0.1.2/tests/test_sourcing_model.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 idinn-0.1.2/.gitignore
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 idinn-0.1.2/LICENSE
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 idinn-0.1.2/README.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 idinn-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 idinn-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 idinn-0.1.3/.readthedocs.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 idinn-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/conf.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0   453134 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/_static/optimization_schematic.png
+-rw-r--r--   0        0        0   243113 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/_static/youtube.png
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/get_started/get_started.rst
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/get_started/installation.rst
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/joss/paper.bib
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/joss/paper.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/api.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/benchmark.rst
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/dual.rst
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/single.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/tutorials/transfer.rst
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/dynamics.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/optimization.rst
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/order.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 idinn-0.1.3/docs/understand/straight.rst
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 idinn-0.1.3/src/idinn/__init__.py
+-rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 idinn-0.1.3/src/idinn/controller.py
+-rw-r--r--   0        0        0    11952 2020-02-02 00:00:00.000000 idinn-0.1.3/src/idinn/sourcing_model.py
+-rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 idinn-0.1.3/tests/test_controller.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 idinn-0.1.3/tests/test_sourcing_model.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 idinn-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 idinn-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 idinn-0.1.3/README.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 idinn-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 idinn-0.1.3/PKG-INFO
```

### Comparing `idinn-0.1.2/.readthedocs.yaml` & `idinn-0.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/docs/Makefile` & `idinn-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/docs/conf.py` & `idinn-0.1.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Import for autodoc -----------------------------------------------------
 
 import os
 import sys
-sys.path.insert(0, os.path.abspath("../"))
+sys.path.insert(0, os.path.abspath("../src/idinn"))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "idinn"
 copyright = "2024, J. Li, T. Asikis, I. Fragkos, L. Böttcher"
 author = "J. Li, T. Asikis, I. Fragkos, L. Böttcher"
```

### Comparing `idinn-0.1.2/docs/index.rst` & `idinn-0.1.3/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 ######################################################
 idinn: Inventory-Dynamics Control with Neural Networks
 ######################################################
 
 ..  youtube:: hUBfTWV6tWQ
    :width: 100%
 
-`idinn` implements inventory dynamics–informed neural networks designed for solving both single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into easily customizable classes, such as :class:`SingleSourcingModel` and :class:`SingleSourcingNeuralController`, to enable users to find the optimal order policies for the user-specified inventory systems.
+`idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
 
 Example Usage
 =============
 
 .. code-block:: python
 
    import torch
    from idinn.sourcing_model import SingleSourcingModel
-   from idinn.controller import SingleFullyConnectedNeuralController
+   from idinn.controller import SingleSourcingNeuralController
 
    # Initialize the sourcing model and the neural controller
    sourcing_model = SingleSourcingModel(
-      lead_time=0, holding_cost=5, shortage_cost=495, batch_size=32, init_inventory=10
+      lead_time=0,
+      holding_cost=5,
+      shortage_cost=495,
+      batch_size=32,
+      init_inventory=10,
+      demand_distribuion="uniform",
+      demand_low=1,
+      demand_high=4
    )
    controller = SingleFullyConnectedNeuralController(
-      hidden_layers=[2], activation=torch.nn.CELU(alpha=1)
+      hidden_layers=[2],
+      activation=torch.nn.CELU(alpha=1)
    )
    # Train the neural controller
    controller.train(
       sourcing_model=sourcing_model,
       sourcing_periods=50,
       validation_sourcing_periods=1000,
       epochs=5000,
       tensorboard_writer=torch.utils.tensorboard.SummaryWriter(),
       seed=1,
    )
    # Simulate and plot the results
    controller.plot(sourcing_model=sourcing_model, sourcing_periods=100)
    # Calculate the optimal order quantity for applications
-   controller.forward(
-      current_inventory=torch.tensor([[10]]),
-      past_orders=torch.tensor([[1, 5]]),
-   )
+   controller.forward(current_inventory=10, past_orders=[1, 5])
 
 .. toctree::
    :hidden:
    :maxdepth: 1
    :caption: Get Started
 
    get_started/installation
@@ -51,22 +56,11 @@
 .. toctree::
    :hidden:
    :maxdepth: 1
    :caption: Tutorials
 
    tutorials/single
    tutorials/dual
-   tutorials/transfer
-   tutorials/benchmark
-
-.. toctree::
-   :hidden:
-   :maxdepth: 1
-   :caption: Understand idinn
+   tutorials/api
 
-   understand/order
-   understand/dynamics
-   understand/straight
-   understand/optimization
-   understand/api
```

### Comparing `idinn-0.1.2/docs/make.bat` & `idinn-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/docs/_static/optimization_schematic.png` & `idinn-0.1.3/docs/_static/optimization_schematic.png`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/docs/_static/youtube.png` & `idinn-0.1.3/docs/_static/youtube.png`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/docs/get_started/get_started.rst` & `idinn-0.1.3/docs/get_started/get_started.rst`

 * *Files 20% similar despite different names*

```diff
@@ -13,24 +13,27 @@
 
    # Initialize the sourcing model
    sourcing_model = SingleSourcingModel(
       lead_time=0,
       holding_cost=5,
       shortage_cost=495,
       batch_size=32,
-      init_inventory=10
+      init_inventory=10,
+      demand_distribuion="uniform",
+      demand_low=1,
+      demand_high=4
    )
 
-Afterwards, initialize a controller that is compatible with the chosen sourcing model. In the above single-sourcing example, the relevant controller is :class:`SingleFullyConnectedNeuralController`.
+Afterwards, initialize a controller that is compatible with the chosen sourcing model. In the above single-sourcing example, the relevant controller is :class:`SingleSourcingNeuralController`.
 
 .. code-block:: python
 
-    from idinn.controller import SingleFullyConnectedNeuralController
+    from idinn.controller import SingleSourcingNeuralController
     # Initialize the neural controller
-    controller = SingleFullyConnectedNeuralController()
+    controller = SingleSourcingNeuralController()
 
 Training
 --------
 
 The selected controller needs to be trained to find the optimal neural-network parameters.
 
 .. code-block:: python
@@ -54,11 +57,8 @@
 
 
 The trained controller can be used for optimal order quantity calculations.
 
 .. code-block:: python
 
    # Calculate the optimal order quantity for applications
-   controller.forward(
-      current_inventory=torch.tensor([[10]]),
-      past_orders=torch.tensor([[1, 5]]),
-   )
+   controller.forward(current_inventory=10, past_orders=[1, 5])
```

### Comparing `idinn-0.1.2/docs/get_started/installation.rst` & `idinn-0.1.3/docs/get_started/installation.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 ************
 Installation
 ************
 
+Install `idinn`
+===============
+
 Requirements
 ============
 
-The basic usage of `idinn` requires a working `Python`_ and `PyTorch`_ installation. If plotting simulation result of a controller is needed, `matplotlib`_ should also be installed. We recommend using the following versions for maximum 
+The basic usage of `idinn` requires a working `Python`_ and `PyTorch`_ installation. If plotting simulation result of a controller is needed, `matplotlib`_ should also be installed. We recommend using the following versions for maximum compability:
 
 * Python_     ``>= 3.8``
 * PyTorch_    ``>= 2.0``
 * matplotlib_ ``>= 3.0``
 
 Install `idinn`
 ===============
 
-The package can be installed form the git repository. To do that, run
+The package can be installed form PyPI. To do that, run
 
 .. code-block::
 
-   python -m pip install git+https://gitlab.com/ComputationalScience/inventory-optimization.git@main
+   pip install idinn
 
 Or, if you want to inspect and locally edit the source code, run
 
 .. code-block::
 
-   git clone https://gitlab.com/ComputationalScience/inventory-optimization.git
-   cd inventory-optimization
-   python -m pip install -e .
+   git clone https://gitlab.com/ComputationalScience/idinn.git
+   cd idinn
+   pip install -e .
 
 .. _Python: https://www.python.org/downloads/
 .. _PyTorch: https://pytorch.org/get-started/locally/
 .. _matplotlib: https://matplotlib.org/stable/users/getting_started/
```

### Comparing `idinn-0.1.2/docs/joss/paper.bib` & `idinn-0.1.3/docs/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/docs/joss/paper.md` & `idinn-0.1.3/docs/joss/paper.md`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/docs/tutorials/dual.rst` & `idinn-0.1.3/docs/tutorials/dual.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 ==================================================
 
 Dual-sourcing problems are similar to single-sourcing problems but are more intricate. In a dual-sourcing problem, a company has two potential suppliers for a product, each offering varying lead times (the duration for orders to arrive) and order costs (the expense of placing an order). The challenge lies in the company's decision-making process: determining which supplier to engage for each product to minimize costs given stochastic demand. We can solve dual-sourcing problems with `idinn` in a way similar to the approaches describes described in :doc:`/get_started/get_started` and :doc:`/tutorials/single`.
 
 Initialization
 --------------
 
-To address dual-sourcing problems, we employ two main classes: `DualSourcingModel` and `DualFullyConnectedNeuralController`, responsible for setting up the sourcing model and its corresponding controller. In this tutorial, we adopt a dual-sourcing model with specific parameters: regular order lead time and expedited order lead time both set to 0, regular order cost, :math:`c^r`, at 0, expedited order cost, :math:`c^e`, at 20, initial inventory of 6, and a batch size of 256. Additionally, the holding cost, :math:`h`, is 5, while the shortage cost, :math:`s`, is 495. Demand is generated from a uniform distribution with the interval :math:`[0, 5)`. Notice that the `high` parameter is exclusive. Hence, the generated demand never exceeds 4. In our code, the sourcing model is initialized as follows.
+To address dual-sourcing problems, we employ two main classes: `DualSourcingModel` and `DualSourcingNeuralController`, responsible for setting up the sourcing model and its corresponding controller. In this tutorial, we adopt a dual-sourcing model with specific parameters: regular order lead time and expedited order lead time both set to 0, regular order cost, :math:`c^r`, at 0, expedited order cost, :math:`c^e`, at 20, initial inventory of 6, and a batch size of 256. Additionally, the holding cost, :math:`h`, is 5, while the shortage cost, :math:`s`, is 495. Demand is generated from a uniform distribution with interval :math:`[0, 4]`. Notice that both the `demand_low` and `demand_low` parameter are inclusive (closed bracket). Hence, the generated demand will never exceed 4. In our code, the sourcing model is initialized as follows.
 
 .. code-block:: python
     
    import torch
    from idinn.sourcing_model import DualSourcingModel
-   from idinn.controller import DualFullyConnectedNeuralController
+   from idinn.controller import DualSourcingNeuralController
 
     dual_sourcing_model = DualSourcingModel(
         regular_lead_time=2,
         expedited_lead_time=0,
         regular_order_cost=0,
         expedited_order_cost=20,
         holding_cost=5,
         shortage_cost=495,
         batch_size=256,
         init_inventory=6,
+        demand_distribuion="uniform",
+        demand_low=1,
+        demand_high=4
     )
 
 The cost at period :math:`t`, :math:`c_t`, is
 
 .. math::
 
    c_t = c^r q^r_t + c^e q^e_t + h \cdot \max(0, I_t) + s \cdot \max(0, - I_t)\,,
@@ -35,19 +38,19 @@
 
 .. code-block:: python
     
    dual_sourcing_model.get_cost(regular_q=0, expedited_q=0)
 
 In our example, this function should return 30 for each sample since the initial inventory is 6, the holding cost is 5, and there is neither a regular nor expedited order. We have 256 samples in this case, as we specified a batch size of 256.
 
-For dual-sourcing problems, we initialize the neural network controller using the `DualFullyConnectedNeuralController` class. In this tutorial, we use a simple neural network with 6 hidden layers and 128, 64, 32, 16, 8, 4 neurons, respectively. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
+For dual-sourcing problems, we initialize the neural network controller using the `DualSourcingNeuralController` class. In this tutorial, we use a simple neural network with 6 hidden layers and 128, 64, 32, 16, 8, 4 neurons, respectively. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
 
 .. code-block:: python
 
-    dual_controller = SingleFullyConnectedNeuralController(
+    dual_controller = DualSourcingNeuralController(
         hidden_layers=[128, 64, 32, 16, 8, 4], activation=torch.nn.CELU(alpha=1)
     )
 
 Training
 --------
 
 Although the neural network controller has not been trained yet, we can still utilize it to calculate the total cost if we apply this controller for 100 periods alongside our previously specified sourcing model.
@@ -84,23 +87,24 @@
 
 .. code-block:: python
 
     # Simulate and plot the results
     dual_controller.plot(sourcing_model=dual_sourcing_model, sourcing_periods=100)
     # Calculate the optimal order quantity for applications
     regular_q, expedited_q = dual_controller.forward(
-        current_inventory=torch.tensor([[10]]),
-        past_regular_orders=torch.tensor([[1, 5]]),
-        past_expedited_orders=torch.tensor([[0, 0]]),
+        current_inventory=10,
+        past_regular_orders=[1, 5],
+        past_expedited_orders=[0, 0],
     )
 
 Save and Load the Model
 -----------------------
 
 It is also a good idea to save the trained neural network controller for future use. This can be done using the `save` method. The `load` method allows one to load a previously saved model.
 
 .. code-block:: python
 
     # Save the model
     dual_controller.save("optimal_dual_sourcing_controller.pt")
     # Load the model
-    dual_controller_loaded = DualFullyConnectedNeuralController().load("optimal_dual_sourcing_controller.pt")
+    dual_controller_loaded = DualSourcingNeuralController()
+    dual_controller_loaded.load("optimal_dual_sourcing_controller.pt")
```

### Comparing `idinn-0.1.2/docs/tutorials/single.rst` & `idinn-0.1.3/docs/tutorials/single.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 ====================================================
 
 Single-sourcing problems are inventory management problems where only one delivery option exists. The overall objective in single-sourcing and related inventory management problems is for companies to identify the optimal order quantities to minimize costs given stochastic demand. This problem can be addressed using `idinn`. As illustrated in the :doc:`/get_started/get_started` section, we first initialize the sourcing model and its associated neural network controller. Subsequently, we train the neural network controller using data generated from the sourcing model. Finally, we can use the trained neural network controller to compute optimal order quantities.
 
 Initialization
 --------------
 
-Since we deal with the single-sourcing problem, we use the `SingleSourcingModel` class to initialize the sourcing model. In this tutorial, let us pick a single sourcing model which has a lead time of 0, i.e. the order arrives immediately after it is placed, an initial inventory of 10 and a batch size of 32. The holding cost, :math:`h`, is 5 and the shortage cost, :math:`s`, is 495. The demand is generated from a uniform distribution with interval :math:`[0, 5)`. Notice that the `high` parameter is exclusive (open bracket). Hence, the generated demand will never exceed 4. In our code, the sourcing model is initialized as follows.
+Since we deal with the single-sourcing problem, we use the `SingleSourcingModel` class to initialize the sourcing model. In this tutorial, let us pick a single sourcing model which has a lead time of 0, i.e. the order arrives immediately after it is placed, an initial inventory of 10 and a batch size of 32. The holding cost, :math:`h`, is 5 and the shortage cost, :math:`s`, is 495. The demand is generated from a uniform distribution with interval :math:`[0, 4]`. Notice that both the `demand_low` and `demand_low` parameter are inclusive (closed bracket). Hence, the generated demand will never exceed 4. In our code, the sourcing model is initialized as follows.
 
 .. code-block:: python
     
    import torch
    from idinn.sourcing_model import SingleSourcingModel
-   from idinn.controller import SingleFullyConnectedNeuralController
+   from idinn.controller import SingleSourcingNeuralController
 
    single_sourcing_model = SingleSourcingModel(
       lead_time=0,
       holding_cost=5,
       shortage_cost=495,
       batch_size=32,
       init_inventory=10,
-      demand_generator=torch.distributions.Uniform(low=0, high=5)
+      demand_distribuion="uniform",
+      demand_low=1,
+      demand_high=4
    )
 
 The cost at period :math:`t`, :math:`c_t`, is
 
 .. math::
 
    c_t = h \cdot \max(0, I_t) + s \cdot \max(0, - I_t)\,,
@@ -33,19 +35,19 @@
 
 .. code-block:: python
     
    single_sourcing_model.get_cost()
 
 In our example, this function should return 50 for each sample since the initial inventory is 10 and the holding cost is 5. We have 32 samples in this case, as we specified a batch size of 32.
 
-For single-sourcing problems, we initialize the neural network controller using the `SingleFullyConnectedNeuralController` class. In this tutorial, we use a simple neural network with 1 hidden layer and 2 neurons. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
+For single-sourcing problems, we initialize the neural network controller using the `SingleSourcingNeuralController` class. In this tutorial, we use a simple neural network with 1 hidden layer and 2 neurons. The activation function is `torch.nn.CELU(alpha=1)`. The neural network controller is initialized as follows.
 
 .. code-block:: python
 
-    single_controller = SingleFullyConnectedNeuralController(
+    single_controller = SingleSourcingNeuralController(
         hidden_layers=[2], activation=torch.nn.CELU(alpha=1)
     )
 
 Training
 --------
 
 Although the neural network controller has not been trained yet, we can still utilize it to calculate the total cost if we apply this controller for 100 periods alongside our previously specified sourcing model.
@@ -81,26 +83,23 @@
 We can also inspect how the controller performs in the specified sourcing environment by (i) plotting the inventory and order histories and (ii) calculating optimal orders.
 
 .. code-block:: python
 
     # Simulate and plot the results
     single_controller.plot(sourcing_model=single_sourcing_model, sourcing_periods=100)
     # Calculate the optimal order quantity for applications
-    single_controller.forward(
-        current_inventory=torch.tensor([[10]]),
-        past_orders=torch.tensor([[1, 5]]),
-    )
+    single_controller.forward(current_inventory=10, past_orders=[1, 5])
 
 Save and Load the Model
 -----------------------
 
-It is also a good idea to save the trained neural network controller for future use. This can be done using the `save` method. The `load` method allows one to load a previously saved model.
+It is also a good idea to save the trained neural network controller for future use. This can be done using the `save` method. The `load` method allows one to load a previously saved controller.
 
 .. code-block:: python
 
     # Save the model
     single_controller.save("optimal_single_sourcing_controller.pt")
     # Load the model
-    single_controller_loaded = SingleFullyConnectedNeuralController(
+    single_controller_loaded = SingleSourcingNeuralController(
         hidden_layers=[2], activation=torch.nn.CELU(alpha=1)
     )
     single_controller_loaded.load("optimal_single_sourcing_controller.pt")
```

### Comparing `idinn-0.1.2/src/idinn/controller.py` & `idinn-0.1.3/src/idinn/controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,54 +13,54 @@
 
 class SingleSourcingNeuralController(torch.nn.Module, NeuralControllerMixIn):
     """
     SingleSourcingNeuralController is a neural network-based controller for inventory optimization in a single-sourcing scenario.
 
     Parameters
     ----------
-    hidden_layers : list
-        List of integers representing the number of units in each hidden layer. Default is [2].
-    activation : torch.nn.Module
-        Activation function to be used in the hidden layers. Default is torch.nn.CELU(alpha=1).
+    hidden_layers : list, default is [2]
+        List of integers representing the number of units in each hidden layer.
+    activation : torch.nn.Module, default is torch.nn.CELU(alpha=1)
+        Activation function to be used in the hidden layers.
 
     Attributes
     ----------
     hidden_layers : list
         List of integers representing the number of units in each hidden layer.
     activation : torch.nn.Module
         Activation function used in the hidden layers.
     stack : torch.nn.Sequential
         Sequential stack of linear layers and activation functions.
 
     Methods
     -------
     init_layers(lead_time)
-        Initializes the layers of the neural network based on the lead time.
+        Initialize the layers of the neural network based on the lead time.
     forward(current_inventory, past_orders)
-        Performs forward pass through the neural network.
+        Perform forward pass through the neural network.
     get_total_cost(sourcing_model, sourcing_periods, seed=None)
-        Calculates the total cost over a given number of sourcing periods.
+        Calculate the total cost over a given number of sourcing periods.
     train(sourcing_model, sourcing_periods, epochs, ...)
-        Trains the neural network controller using the sourcing model and specified parameters.
+        Train the neural network controller using the sourcing model and specified parameters.
     simulate(sourcing_model, sourcing_periods)
-        Simulates the inventory and order quantities over a given number of sourcing periods.
+        Simulate the inventory and order quantities over a given number of sourcing periods.
     plot(sourcing_model, sourcing_periods)
-        Plots the inventory and order quantities over a given number of sourcing periods.
+        Plot the inventory and order quantities over a given number of sourcing periods.
     """
 
     def __init__(self, hidden_layers=[2], activation=torch.nn.CELU(alpha=1)):
         super().__init__()
         self.hidden_layers = hidden_layers
         self.activation = activation
         self.lead_time = None
         self.stack = None
 
     def init_layers(self, lead_time):
         """
-        Initializes the layers of the neural network based on the lead time.
+        Initialize the layers of the neural network based on the lead time.
 
         Parameters
         ----------
         lead_time : int
             The lead time for sourcing.
 
         Returns
@@ -86,48 +86,50 @@
 
     def forward(
         self,
         current_inventory,
         past_orders,
     ):
         """
-        Performs forward pass through the neural network.
+        Perform forward pass through the neural network.
 
         Parameters
         ----------
-        current_inventory : torch.Tensor
+        current_inventory : int, or torch.Tensor
             Current inventory levels.
-        past_orders : torch.Tensor
+        past_orders : int, or torch.Tensor
             Past order quantities.
 
         Returns
         -------
         torch.Tensor
-            Predicted order quantities.
+            Order quanty calculated by the neural network.
         """
+        if not isinstance(current_inventory, torch.Tensor):
+            current_inventory = torch.tensor([[current_inventory]], dtype=torch.float32)
+        if not isinstance(past_orders, torch.Tensor):
+            past_orders = torch.tensor([past_orders], dtype=torch.float32)
         if self.lead_time > 0:
             h = torch.cat([current_inventory, past_orders[:, -self.lead_time :]], dim=1)
-        else:
-            h = current_inventory
         h = self.stack(h)
         q = h - torch.frac(h).clone().detach()
         return q
 
     def get_total_cost(self, sourcing_model, sourcing_periods, seed=None):
         """
-        Calculates the total cost over a given number of sourcing periods.
+        Calculate the total cost over a given number of sourcing periods.
 
         Parameters
         ----------
         sourcing_model : SourcingModel
             The sourcing model to be used for cost calculation.
         sourcing_periods : int
             The number of sourcing periods.
         seed : int, optional
-            Random seed for reproducibility. Default is None.
+            Random seed for reproducibility.
 
         Returns
         -------
         numpy.ndarray
             Total cost over the sourcing periods.
         """
         if seed is not None:
@@ -154,38 +156,34 @@
         validation_sourcing_periods=None,
         lr_init_inventory=1e-1,
         lr_parameters=3e-3,
         seed=None,
         tensorboard_writer=None,
     ):
         """
-        Trains the neural network controller using the sourcing model and specified parameters.
+        Train the neural network controller using the sourcing model and specified parameters.
 
         Parameters
         ----------
         sourcing_model : SourcingModel
             The sourcing model to be used for training.
         sourcing_periods : int
             The number of sourcing periods for training.
         epochs : int
             The number of training epochs.
         validation_sourcing_periods : int, optional
-            The number of sourcing periods for validation. Default is None.
-        lr_init_inventory : float, optional
-            Learning rate for initializing inventory. Default is 1e-1.
-        lr_parameters : float, optional
-            Learning rate for updating neural network parameters. Default is 3e-3.
+            The number of sourcing periods for validation.
+        lr_init_inventory : float, default is 1e-1
+            Learning rate for initial inventory.
+        lr_parameters : float, default is 3e-3
+            Learning rate for updating neural network parameters. 
         seed : int, optional
-            Random seed for reproducibility. Default is None.
+            Random seed for reproducibility.
         tensorboard_writer : tensorboard.SummaryWriter, optional
-            Tensorboard writer for logging. Default is None.
-
-        Returns
-        -------
-        None
+            Tensorboard writer for logging.
         """
         if seed is not None:
             torch.manual_seed(seed)
 
         optimizer_init_inventory = torch.optim.RMSprop(
             [sourcing_model.init_inventory], lr=lr_init_inventory
         )
@@ -234,24 +232,24 @@
                     )
                 tensorboard_writer.flush()
         # Load the best model
         self.load_state_dict(best_state)
 
     def simulate(self, sourcing_model, sourcing_periods, seed=None):
         """
-        Simulates the inventory and order quantities over a given number of sourcing periods.
+        Simulate the inventory and order quantities over a given number of sourcing periods.
 
         Parameters
         ----------
-        sourcing_model : SourcingModel
+        sourcing_model : SingleSourcingModel
             The sourcing model to be used for simulation.
         sourcing_periods : int
             The number of sourcing periods for simulation.
         seed : int, optional
-            Random seed for reproducibility. Default is None.
+            Random seed for reproducibility.
 
         Returns
         -------
         tuple
             A tuple containing the past inventories and past orders as numpy arrays.
         """
         if seed is not None:
@@ -264,26 +262,22 @@
             sourcing_model.order(q)
         past_inventories = sourcing_model.get_past_inventories()[0, :].detach().numpy()
         past_orders = sourcing_model.get_past_orders()[0, :].detach().numpy()
         return past_inventories, past_orders
 
     def plot(self, sourcing_model, sourcing_periods):
         """
-        Plots the inventory and order quantities over a given number of sourcing periods.
+        Plot the inventory and order quantities over a given number of sourcing periods.
 
         Parameters
         ----------
-        sourcing_model : SourcingModel
+        sourcing_model : SingleSourcingModel
             The sourcing model to be used for plotting.
         sourcing_periods : int
             The number of sourcing periods for plotting.
-
-        Returns
-        -------
-        None
         """
         past_inventories, past_orders = self.simulate(
             sourcing_model=sourcing_model, sourcing_periods=sourcing_periods
         )
         fig, ax = plt.subplots(ncols=2, figsize=(10, 4))
 
         ax[0].step(range(sourcing_periods), past_inventories[-sourcing_periods:])
@@ -301,19 +295,19 @@
 
 class DualSourcingNeuralController(torch.nn.Module, NeuralControllerMixIn):
     """
     DualSourcingNeuralController is a neural network controller for dual sourcing inventory optimization.
 
     Parameters
     ----------
-    hidden_layers : list
+    hidden_layers : list, default is [128, 64, 32, 16, 8, 4]
         List of integers specifying the sizes of hidden layers.
-    activation : torch.nn.Module
+    activation : torch.nn.Module, default is torch.nn.CELU(alpha=1)
         Activation function to be used in the hidden layers.
-    compressed : bool
+    compressed : bool, default is False
         Flag indicating whether the input is compressed.
 
     Attributes
     ----------
     hidden_layers : list
         List of integers specifying the sizes of hidden layers.
     activation : torch.nn.Module
@@ -331,16 +325,16 @@
     -------
     init_layers(regular_lead_time, expedited_lead_time)
         Initialize the layers of the neural network.
     forward(current_inventory, past_orders)
         Forward pass of the neural network.
     get_total_cost(sourcing_model, sourcing_periods, seed=None)
         Calculate the total cost of the sourcing model.
-    train(sourcing_model, sourcing_periods, epochs, validation_sourcing_periods=None, lr_init_inventory=1e-1, lr_parameters=3e-3, seed=None, tensorboard_writer=None)
-        Train the neural network.
+    train(sourcing_model, sourcing_periods, epochs, ...)
+        Trains the neural network controller using the sourcing model and specified parameters.
     simulate(sourcing_model, sourcing_periods, seed=None)
         Simulate the sourcing model using the neural network.
     plot(sourcing_model, sourcing_periods)
         Plot the inventory and order quantities.
     """
 
     def __init__(
@@ -362,18 +356,14 @@
 
         Parameters
         ----------
         regular_lead_time : int
             Regular lead time.
         expedited_lead_time : int
             Expedited lead time.
-
-        Returns
-        -------
-        None
         """
         self.regular_lead_time = regular_lead_time
         self.expedited_lead_time = expedited_lead_time
         if self.compressed:
             input_length = regular_lead_time + expedited_lead_time
         else:
             input_length = regular_lead_time + expedited_lead_time + 1
@@ -396,28 +386,35 @@
 
     def forward(self, current_inventory, past_regular_orders, past_expedited_orders):
         """
         Forward pass of the neural network.
 
         Parameters
         ----------
-        current_inventory : torch.Tensor
+        current_inventory : int, or torch.Tensor
             Current inventory.
-        past_regular_orders : torch.Tensor
+        past_regular_orders : int, or torch.Tensor
             Past regular orders.
-        past_expedited_orders : torch.Tensor
+        past_expedited_orders : int, or torch.Tensor
             Past expedited orders.
 
         Returns
         -------
         regular_q : torch.Tensor
             Regular order quantity.
         expedited_q : torch.Tensor
             Expedited order quantity.
         """
+        if not isinstance(current_inventory, torch.Tensor):
+            current_inventory = torch.tensor([[current_inventory]], dtype=torch.float32)
+        if not isinstance(past_regular_orders, torch.Tensor):
+            past_regular_orders = torch.tensor([past_regular_orders], dtype=torch.float32)
+        if not isinstance(past_expedited_orders, torch.Tensor):
+            past_expedited_orders = torch.tensor([past_expedited_orders], dtype=torch.float32)
+
         if self.regular_lead_time > 0:
             if self.compressed:
                 inputs = past_regular_orders[:, -self.regular_lead_time :]
                 inputs[:, 0] += current_inventory
             else:
                 inputs = torch.cat(
                     [
@@ -440,16 +437,16 @@
 
     def get_total_cost(self, sourcing_model, sourcing_periods, seed=None):
         """
         Calculate the total cost of the sourcing model.
 
         Parameters
         ----------
-        sourcing_model : Sourcing model.
-            Sourcing model.
+        sourcing_model : DualSourcingModel
+            The sourcing model.
         sourcing_periods : int
             Number of sourcing periods.
         seed : int, optional
             Random seed for reproducibility.
 
         Returns
         -------
@@ -490,26 +487,26 @@
         tensorboard_writer=None,
     ):
         """
         Train the neural network.
 
         Parameters
         ----------
-        sourcing_model : Sourcing model
-            Sourcing model.
+        sourcing_model : DualSourcingModel
+            The sourcing model.
         sourcing_periods : int
             Number of sourcing periods.
         epochs : int
             Number of training epochs.
         validation_sourcing_periods : int, optional
             Number of sourcing periods for validation.
-        lr_init_inventory : float, optional
-            Learning rate for initializing inventory.
-        lr_parameters : float, optional
-            Learning rate for neural network parameters.
+        lr_init_inventory : float, default is 1e-1
+            Learning rate for initial inventory.
+        lr_parameters : float, default is 3e-3
+            Learning rate for updating neural network parameters.
         seed : int, optional
             Random seed for reproducibility.
         tensorboard_writer : TensorBoard writer, optional
             TensorBoard writer for logging.
         """
         if seed is not None:
             torch.manual_seed(seed)
@@ -562,15 +559,15 @@
 
     def simulate(self, sourcing_model, sourcing_periods, seed=None):
         """
         Simulate the sourcing model using the neural network.
 
         Parameters
         ----------
-        sourcing_model : Sourcing model
+        sourcing_model : DualSourcingModel
             The sourcing model.
         sourcing_periods : int
             Number of sourcing periods.
         seed : int, optional
             Random seed for reproducibility.
 
         Returns
@@ -605,311 +602,15 @@
 
     def plot(self, sourcing_model, sourcing_periods):
         """
         Plot the inventory and order quantities.
 
         Parameters
         ----------
-        sourcing_model : Sourcing model
-            The sourcing model.
-        sourcing_periods : int
-            Number of sourcing periods.
-
-        Returns
-        -------
-        None
-
-        """
-        past_inventories, past_regular_orders, past_expedited_orders = self.simulate(
-            sourcing_model=sourcing_model, sourcing_periods=sourcing_periods
-        )
-        fig, ax = plt.subplots(ncols=2, figsize=(10, 4))
-        ax[0].step(range(sourcing_periods), past_inventories[-sourcing_periods:])
-        ax[0].yaxis.get_major_locator().set_params(integer=True)
-        ax[0].set_title("Inventory")
-        ax[0].set_xlabel("Period")
-        ax[0].set_ylabel("Quantity")
-
-        ax[1].step(
-            range(sourcing_periods),
-            past_expedited_orders[-sourcing_periods:],
-            label="Expedited Order",
-        )
-        ax[1].step(
-            range(sourcing_periods),
-            past_regular_orders[-sourcing_periods:],
-            label="Regular Order",
-        )
-        ax[1].yaxis.get_major_locator().set_params(integer=True)
-        ax[1].set_title("Order")
-        ax[1].set_xlabel("Period")
-        ax[1].set_ylabel("Quantity")
-        ax[1].legend()
-
-
-class CappedDualIndexController:
-    """
-    Controller class for capped dual index inventory optimization.
-
-    Parameters
-    ----------
-    s_e : int
-        Capped dual index parameter 1
-    s_r : int
-        Capped dual index parameter 2
-    q_r : int
-        Capped dual index parameter 3
-
-    Notes
-    -----
-    The function follows the implementation of Sun, J., & Van Mieghem, J. A. (2019)([1]_).
-
-    References
-    ----------
-    .. [1] Robust dual sourcing inventory management: Optimality of capped dual index policies and smoothing.
-           Manufacturing & Service Operations Management, 21(4), 912-931.
-    """
-
-    def __init__(self, s_e=0, s_r=0, q_r=0):
-        self.s_e = s_e
-        self.s_r = s_r
-        self.q_r = q_r
-
-    def capped_dual_index_sum(
-        self,
-        current_inventory,
-        past_regular_orders,
-        past_expedited_orders,
-        regular_lead_time,
-        expedited_lead_time,
-        k,
-    ):
-        """
-        Calculate the capped dual index sum.
-
-        Parameters
-        ----------
-        current_inventory : int
-            Current inventory level.
-        past_regular_orders : numpy.ndarray
-            Array of past regular orders.
-        past_expedited_orders : numpy.ndarray
-            Array of past expedited orders.
-        regular_lead_time : int
-            Regular lead time.
-        expedited_lead_time : int
-            Expedited lead time.
-        k : int
-            Parameter for capped dual index sum calculation.
-
-        Returns
-        -------
-        int
-            The capped dual index sum.
-        """
-        inventory_position = (
-            current_inventory
-            + past_regular_orders[
-                :, -regular_lead_time : -regular_lead_time + k + 1
-            ].sum()
-        )
-        if expedited_lead_time > max(1, expedited_lead_time - k):
-            inventory_position += past_expedited_orders[
-                -expedited_lead_time : -expedited_lead_time
-                + min(k, expedited_lead_time - 1)
-                + 1
-            ].sum()
-        return inventory_position
-
-    def forward(
-        self,
-        current_inventory,
-        past_regular_orders,
-        past_expedited_orders,
-        regular_lead_time,
-        expedited_lead_time,
-    ):
-        """
-        Perform forward calculation for capped dual index optimization.
-
-        Parameters
-        ----------
-        current_inventory : int
-            Current inventory level.
-        past_regular_orders : numpy.ndarray
-            Array of past regular orders.
-        past_expedited_orders : numpy.ndarray
-            Array of past expedited orders.
-        regular_lead_time : int
-            Regular lead time.
-        expedited_lead_time : int
-            Expedited lead time.
-
-        Returns
-        -------
-        tuple
-            A tuple containing the regular order quantity and expedited order quantity.
-        """
-        inventory_position = self.capped_dual_index_sum(
-            current_inventory,
-            past_regular_orders,
-            past_expedited_orders,
-            regular_lead_time,
-            expedited_lead_time,
-            k=0,
-        )
-        inventory_position_limit = self.capped_dual_index_sum(
-            current_inventory,
-            past_regular_orders,
-            past_expedited_orders,
-            regular_lead_time,
-            expedited_lead_time,
-            k=regular_lead_time - expedited_lead_time - 1,
-        )
-        regular_q = min(max(0, self.s_r - inventory_position_limit), self.q_r)
-        expedited_q = max(0, self.s_e - inventory_position)
-        return regular_q, expedited_q
-
-    def get_total_cost(self, sourcing_model, sourcing_periods, seed=None):
-        """
-        Calculate the total cost for capped dual index optimization.
-
-        Parameters
-        ----------
-        sourcing_model : SourcingModel
-            The sourcing model.
-        sourcing_periods : int
-            Number of sourcing periods.
-        seed : int, optional
-            Random seed for reproducibility.
-
-        Returns
-        -------
-        float
-            The total cost.
-        """
-        if seed is not None:
-            torch.manual_seed(seed)
-        regular_lead_time = sourcing_model.get_regular_lead_time()
-        expedited_lead_time = sourcing_model.get_expedited_lead_time()
-        total_cost = 0
-        for i in range(sourcing_periods):
-            current_inventory = sourcing_model.get_current_inventory()
-            past_regular_orders = sourcing_model.get_past_regular_orders()
-            past_expedited_orders = sourcing_model.get_past_expedited_orders()
-            regular_q, expedited_q = self.forward(
-                current_inventory,
-                past_regular_orders,
-                past_expedited_orders,
-                regular_lead_time,
-                expedited_lead_time,
-            )
-            sourcing_model.order(regular_q, expedited_q)
-            current_cost = sourcing_model.get_cost(regular_q, expedited_q)
-            total_cost += current_cost
-        return total_cost
-
-    def train(
-        self,
-        sourcing_model,
-        sourcing_periods,
-        s_e_range=np.arange(2, 11),
-        s_r_range=np.arange(2, 11),
-        q_r_range=np.arange(2, 11),
-        seed=None,
-    ):
-        """
-        Train the capped dual index controller.
-
-        Parameters
-        ----------
-        sourcing_model : SourcingModel
-            The sourcing model.
-        sourcing_periods : int
-            Number of sourcing periods.
-        s_e_range : numpy.ndarray, optional
-            Range of values for s_e.
-        s_r_range : numpy.ndarray, optional
-            Range of values for s_r.
-        q_r_range : numpy.ndarray, optional
-            Range of values for q_r.
-        seed : int, optional
-            Random seed for reproducibility.
-        """
-        if seed is not None:
-            torch.manual_seed(seed)
-        min_cost = np.inf
-        for s_e in s_e_range:
-            for s_r in s_r_range:
-                for q_r in q_r_range:
-                    sourcing_model.reset()
-                    self.s_e = s_e
-                    self.s_r = s_r
-                    self.q_r = q_r
-                    total_cost = self.get_total_cost(sourcing_model, sourcing_periods)
-                    if total_cost < min_cost:
-                        min_cost = total_cost
-                        s_e_optimal = s_e
-                        s_r_optimal = s_r
-                        q_r_optimal = q_r
-        self.s_e = s_e_optimal
-        self.s_r = s_r_optimal
-        self.q_r = q_r_optimal
-
-    def simulate(self, sourcing_model, sourcing_periods, seed=None):
-        """
-        Simulate the capped dual index controller.
-
-        Parameters
-        ----------
-        sourcing_model : SourcingModel
-            The sourcing model.
-        sourcing_periods : int
-            Number of sourcing periods.
-        seed : int, optional
-            Random seed for reproducibility.
-
-        Returns
-        -------
-        tuple
-            A tuple containing the past inventories, past regular orders, and past expedited orders.
-        """
-        if seed is not None:
-            torch.manual_seed(seed)
-        sourcing_model.reset()
-        regular_lead_time = sourcing_model.get_regular_lead_time()
-        expedited_lead_time = sourcing_model.get_expedited_lead_time()
-        for i in range(sourcing_periods):
-            current_inventory = sourcing_model.get_current_inventory()
-            past_regular_orders = sourcing_model.get_past_regular_orders()
-            past_expedited_orders = sourcing_model.get_past_expedited_orders()
-            regular_q, expedited_q = self.forward(
-                current_inventory,
-                past_regular_orders,
-                past_expedited_orders,
-                regular_lead_time,
-                expedited_lead_time,
-            )
-            sourcing_model.order(regular_q, expedited_q)
-        past_inventories = sourcing_model.get_past_inventories()[0, :].detach().numpy()
-        past_regular_orders = (
-            sourcing_model.get_past_regular_orders()[0, :].detach().numpy()
-        )
-        past_expedited_orders = (
-            sourcing_model.get_past_expedited_orders()[0, :].detach().numpy()
-        )
-        return past_inventories, past_regular_orders, past_expedited_orders
-
-    def plot(self, sourcing_model, sourcing_periods):
-        """
-        Plot the simulation results.
-
-        Parameters
-        ----------
-        sourcing_model : SourcingModel
+        sourcing_model : DualSourcingModel
             The sourcing model.
         sourcing_periods : int
             Number of sourcing periods.
         """
         past_inventories, past_regular_orders, past_expedited_orders = self.simulate(
             sourcing_model=sourcing_model, sourcing_periods=sourcing_periods
         )
@@ -930,8 +631,8 @@
             past_regular_orders[-sourcing_periods:],
             label="Regular Order",
         )
         ax[1].yaxis.get_major_locator().set_params(integer=True)
         ax[1].set_title("Order")
         ax[1].set_xlabel("Period")
         ax[1].set_ylabel("Quantity")
-        ax[1].legend()
+        ax[1].legend()
```

### Comparing `idinn-0.1.2/.gitignore` & `idinn-0.1.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -158,7 +158,13 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # VS Code and macOS
 .vscode
 .DS_Store
+
+# Jupyter notebooks
+*.ipynb
+
+# PyTorch checkpoints
+*.pt
```

### Comparing `idinn-0.1.2/LICENSE` & `idinn-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/README.md` & `idinn-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 # idinn: Inventory-Dynamics Control with Neural Networks
 
 [<img src="https://gitlab.com/ComputationalScience/idinn/-/raw/main/docs/_static/youtube.png" align="center" width="60%" size="auto" alt="youtube">](https://www.youtube.com/watch?v=hUBfTWV6tWQ)
 
-`idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into easily customizable classes to enable users to find the optimal controllers for the user-specified inventory systems.
-
-## Requirements
-
-The basic usage of `idinn` requires working `Python` and `PyTorch` installation. If plotting simulation result of a controller is needed, `matplotlib` should also be installed.
+`idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
 
 ## Installation
 
-The package can be installed form the git repository. To do that, run
+The package can be installed form PyPI. To do that, run
 
 ```
-python -m pip install git+https://gitlab.com/ComputationalScience/inventory-optimization.git@main
+pip install idinn
 ```
 
 Or, if you want to inspect the source code and edit locally, run
 
 ```
-git clone https://gitlab.com/ComputationalScience/inventory-optimization.git
-cd inventory-optimization
-python -m pip install -e .
+git clone https://gitlab.com/ComputationalScience/idinn.git
+cd idinn
+pip install -e .
 ```
 
 ## Example Usage
 
 ```python
 import torch
 from idinn.sourcing_model import SingleSourcingModel
-from idinn.controller import SingleFullyConnectedNeuralController
+from idinn.controller import SingleSourcingNeuralController
 
 # Initialize the sourcing model and the neural controller
 sourcing_model = SingleSourcingModel(
-    lead_time=0, holding_cost=5, shortage_cost=495, batch_size=32, init_inventory=10
+    lead_time=0,
+    holding_cost=5,
+    shortage_cost=495,
+    batch_size=32,
+    init_inventory=10,
+    demand_distribuion="uniform",
+    demand_low=1,
+    demand_high=4
 )
 controller = SingleFullyConnectedNeuralController(
-    hidden_layers=[2], activation=torch.nn.CELU(alpha=1)
+    hidden_layers=[2],
+    activation=torch.nn.CELU(alpha=1)
 )
 # Train the neural controller
 controller.train(
     sourcing_model=sourcing_model,
     sourcing_periods=50,
     validation_sourcing_periods=1000,
     epochs=5000,
     tensorboard_writer=torch.utils.tensorboard.SummaryWriter(),
     seed=1,
 )
 # Simulate and plot the results
 controller.plot(sourcing_model=sourcing_model, sourcing_periods=100)
 # Calculate the optimal order quantity for applications
-controller.forward(
-    current_inventory=torch.tensor([[10]]),
-    past_orders=torch.tensor([[1, 5]]),
-)
+controller.forward(current_inventory=10, past_orders=[1, 5])
 ```
 
 ## Documentation
 
 For tutorials and documentation, please refer to our [documentation](https://inventory-optimization.readthedocs.io/en/latest/).
 
 ## Papers using `idinn`
 
-We will add papers that use `ìdinn` to this list as they appear online.
-
 * Böttcher, Lucas, Thomas Asikis, and Ioannis Fragkos. "Control of Dual-Sourcing Inventory Systems Using Recurrent Neural Networks." [INFORMS Journal on Computing](https://pubsonline.informs.org/doi/abs/10.1287/ijoc.2022.0136) 35.6 (2023): 1308-1328.
 
 ## Contributors
 
 * [Jiawei Li](https://github.com/iewaij)
 * [Thomas Asikis](https://gitlab.com/asikist)
 * [Ioannis Fragkos](https://gitlab.com/ioannis.fragkos1)
```

### Comparing `idinn-0.1.2/pyproject.toml` & `idinn-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idinn-0.1.2/PKG-INFO` & `idinn-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idinn
-Version: 0.1.2
+Version: 0.1.3
 Summary: Inventory dynamics–informed neural networks for solving single-sourcing and dual-sourcing problems.
 Project-URL: Homepage, https://gitlab.com/ComputationalScience/idinn
 Project-URL: Documentation, https://inventory-optimization.readthedocs.io
 Project-URL: Issues, https://gitlab.com/ComputationalScience/idinn/-/issues
 Author-email: Jiawei Li <sud.concept0x@icloud.com>, Thomas Asikis <thomas.asikis@uzh.ch>, Ioannis Fragkos <fragkos@rsm.nl>, Lucas Boettcher <l.boettcher@fs.de>
 License: MIT License
         
@@ -40,76 +40,75 @@
 Requires-Dist: numba; extra == 'dynamic-programming'
 Description-Content-Type: text/markdown
 
 # idinn: Inventory-Dynamics Control with Neural Networks
 
 [<img src="https://gitlab.com/ComputationalScience/idinn/-/raw/main/docs/_static/youtube.png" align="center" width="60%" size="auto" alt="youtube">](https://www.youtube.com/watch?v=hUBfTWV6tWQ)
 
-`idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into easily customizable classes to enable users to find the optimal controllers for the user-specified inventory systems.
-
-## Requirements
-
-The basic usage of `idinn` requires working `Python` and `PyTorch` installation. If plotting simulation result of a controller is needed, `matplotlib` should also be installed.
+`idinn` implements **i**nventory **d**ynamics–**i**nformed **n**eural **n**etworks for solving single-sourcing and dual-sourcing problems. Neural network controllers and inventory dynamics are implemented into customizable objects with PyTorch backend to enable users to find the optimal neural controllers for the user-specified inventory systems.
 
 ## Installation
 
-The package can be installed form the git repository. To do that, run
+The package can be installed form PyPI. To do that, run
 
 ```
-python -m pip install git+https://gitlab.com/ComputationalScience/inventory-optimization.git@main
+pip install idinn
 ```
 
 Or, if you want to inspect the source code and edit locally, run
 
 ```
-git clone https://gitlab.com/ComputationalScience/inventory-optimization.git
-cd inventory-optimization
-python -m pip install -e .
+git clone https://gitlab.com/ComputationalScience/idinn.git
+cd idinn
+pip install -e .
 ```
 
 ## Example Usage
 
 ```python
 import torch
 from idinn.sourcing_model import SingleSourcingModel
-from idinn.controller import SingleFullyConnectedNeuralController
+from idinn.controller import SingleSourcingNeuralController
 
 # Initialize the sourcing model and the neural controller
 sourcing_model = SingleSourcingModel(
-    lead_time=0, holding_cost=5, shortage_cost=495, batch_size=32, init_inventory=10
+    lead_time=0,
+    holding_cost=5,
+    shortage_cost=495,
+    batch_size=32,
+    init_inventory=10,
+    demand_distribuion="uniform",
+    demand_low=1,
+    demand_high=4
 )
 controller = SingleFullyConnectedNeuralController(
-    hidden_layers=[2], activation=torch.nn.CELU(alpha=1)
+    hidden_layers=[2],
+    activation=torch.nn.CELU(alpha=1)
 )
 # Train the neural controller
 controller.train(
     sourcing_model=sourcing_model,
     sourcing_periods=50,
     validation_sourcing_periods=1000,
     epochs=5000,
     tensorboard_writer=torch.utils.tensorboard.SummaryWriter(),
     seed=1,
 )
 # Simulate and plot the results
 controller.plot(sourcing_model=sourcing_model, sourcing_periods=100)
 # Calculate the optimal order quantity for applications
-controller.forward(
-    current_inventory=torch.tensor([[10]]),
-    past_orders=torch.tensor([[1, 5]]),
-)
+controller.forward(current_inventory=10, past_orders=[1, 5])
 ```
 
 ## Documentation
 
 For tutorials and documentation, please refer to our [documentation](https://inventory-optimization.readthedocs.io/en/latest/).
 
 ## Papers using `idinn`
 
-We will add papers that use `ìdinn` to this list as they appear online.
-
 * Böttcher, Lucas, Thomas Asikis, and Ioannis Fragkos. "Control of Dual-Sourcing Inventory Systems Using Recurrent Neural Networks." [INFORMS Journal on Computing](https://pubsonline.informs.org/doi/abs/10.1287/ijoc.2022.0136) 35.6 (2023): 1308-1328.
 
 ## Contributors
 
 * [Jiawei Li](https://github.com/iewaij)
 * [Thomas Asikis](https://gitlab.com/asikist)
 * [Ioannis Fragkos](https://gitlab.com/ioannis.fragkos1)
```

