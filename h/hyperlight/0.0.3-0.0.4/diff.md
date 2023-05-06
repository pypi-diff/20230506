# Comparing `tmp/hyperlight-0.0.3.tar.gz` & `tmp/hyperlight-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperlight-0.0.3.tar", max compression
+gzip compressed data, was "hyperlight-0.0.4.tar", max compression
```

## Comparing `hyperlight-0.0.3.tar` & `hyperlight-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10173 2023-04-30 17:07:30.205256 hyperlight-0.0.3/LICENSE
--rw-r--r--   0        0        0    11271 2023-05-01 15:53:46.590356 hyperlight-0.0.3/README.md
--rw-r--r--   0        0        0      180 2023-05-01 15:54:36.126996 hyperlight-0.0.3/hyperlight/__init__.py
--rw-r--r--   0        0        0     6320 2023-04-30 17:16:14.247970 hyperlight-0.0.3/hyperlight/convert.py
--rw-r--r--   0        0        0     4101 2023-05-01 13:50:40.802147 hyperlight-0.0.3/hyperlight/find.py
--rw-r--r--   0        0        0       43 2023-04-30 17:07:30.229256 hyperlight-0.0.3/hyperlight/hypernet/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-30 17:07:30.233256 hyperlight-0.0.3/hyperlight/hypernet/encoding.py
--rw-r--r--   0        0        0     3624 2023-04-30 17:07:30.237256 hyperlight-0.0.3/hyperlight/hypernet/initialization.py
--rw-r--r--   0        0        0    13483 2023-05-01 15:11:47.669858 hyperlight-0.0.3/hyperlight/hypernet/model.py
--rw-r--r--   0        0        0      141 2023-04-30 17:07:30.241256 hyperlight-0.0.3/hyperlight/nn/__init__.py
--rw-r--r--   0        0        0      566 2023-04-30 17:07:30.245257 hyperlight-0.0.3/hyperlight/nn/container.py
--rw-r--r--   0        0        0     3888 2023-04-30 17:07:30.245257 hyperlight-0.0.3/hyperlight/nn/layers.py
--rw-r--r--   0        0        0     9494 2023-05-01 15:35:13.143976 hyperlight-0.0.3/hyperlight/nn/module.py
--rw-r--r--   0        0        0     4446 2023-04-30 17:07:30.253257 hyperlight-0.0.3/hyperlight/nn/xparam.py
--rw-r--r--   0        0        0     1442 2023-05-01 15:54:34.050969 hyperlight-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    12096 1970-01-01 00:00:00.000000 hyperlight-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-04-30 17:07:30.205256 hyperlight-0.0.4/LICENSE
+-rw-r--r--   0        0        0    13145 2023-05-06 20:41:23.110335 hyperlight-0.0.4/README.md
+-rw-r--r--   0        0        0      180 2023-05-06 20:42:46.131398 hyperlight-0.0.4/hyperlight/__init__.py
+-rw-r--r--   0        0        0     6320 2023-04-30 17:16:14.247970 hyperlight-0.0.4/hyperlight/convert.py
+-rw-r--r--   0        0        0     4101 2023-05-01 13:50:40.802147 hyperlight-0.0.4/hyperlight/find.py
+-rw-r--r--   0        0        0       43 2023-04-30 17:07:30.229256 hyperlight-0.0.4/hyperlight/hypernet/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-30 17:07:30.233256 hyperlight-0.0.4/hyperlight/hypernet/encoding.py
+-rw-r--r--   0        0        0     3624 2023-04-30 17:07:30.237256 hyperlight-0.0.4/hyperlight/hypernet/initialization.py
+-rw-r--r--   0        0        0    15628 2023-05-06 20:41:05.214106 hyperlight-0.0.4/hyperlight/hypernet/model.py
+-rw-r--r--   0        0        0      141 2023-04-30 17:07:30.241256 hyperlight-0.0.4/hyperlight/nn/__init__.py
+-rw-r--r--   0        0        0      566 2023-04-30 17:07:30.245257 hyperlight-0.0.4/hyperlight/nn/container.py
+-rw-r--r--   0        0        0     3888 2023-04-30 17:07:30.245257 hyperlight-0.0.4/hyperlight/nn/layers.py
+-rw-r--r--   0        0        0     9494 2023-05-01 15:35:13.143976 hyperlight-0.0.4/hyperlight/nn/module.py
+-rw-r--r--   0        0        0     4446 2023-04-30 17:07:30.253257 hyperlight-0.0.4/hyperlight/nn/xparam.py
+-rw-r--r--   0        0        0     1442 2023-05-06 20:42:46.127397 hyperlight-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    13904 1970-01-01 00:00:00.000000 hyperlight-0.0.4/PKG-INFO
```

### Comparing `hyperlight-0.0.3/LICENSE` & `hyperlight-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/README.md` & `hyperlight-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,311 +1,377 @@
 # HyperLight
 
-> Hypernetworks in Pytorch made easy
+_Hypernetworks in Pytorch made easy_
 
 [![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&amp;logo=PyTorch&amp;logoColor=white)](https://pytorch.org)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/hyperlight)](https://pypi.org/project/hyperlight/) 
 [![PyPI version](https://badge.fury.io/py/hyperlight.svg)](https://badge.fury.io/py/hyperlight)
 [![Downloads](https://pepy.tech/badge/hyperlight)](https://pepy.tech/project/hyperlight)
 [![license](https://img.shields.io/github/license/JJGO/hyperlight.svg)](https://github.com/JJGO/hyperlight/blob/main/LICENSE)
 
+
 ## TL;DR
 
 HyperLight is a Pytorch library designed to make implementing hypernetwork models easy and painless.
 What sets HyperLight apart from other hypernetwork implementations:
 
-- **Bring your own architecture** – HyperLight lets you reuse your existing model code.
+- **Bring your own architecture** – Reuse your existing model code.
 - **Principled Parametrizations and Initializations** – Default networks can have unstable training dynamics, HyperLight has good defaults that lead to improved training [1].
-- **Work with pretrained models** – Pretrained weights can be used as part of the hypernetwork initialization.
-- **Seemless Composability** – It's hypernets all the way down! You can hypernetize hypernet models without issue.
-- **_Pytorch-nic_ API design** – Parameters are not treated as inputs to layers, preventing lots of code rewriting from happening.
+- **Work with pretrained models** – Use pretrained weights as part of the hypernetwork initialization.
+- **Seamless Composability** – It's hypernets all the way down! Hypernetize hypernet models without issue.
+- **_Pytorch-nic_ API design** – Parameters are treated as an attribute of the layer, preventing the need for rewriting PyTorch modules.
 <!-- - **Easy weight reuse** – Once a model has its weights set, it can be used many times. -->
+<br>
+<img src="https://raw.githubusercontent.com/JJGO/hyperlight/assets/hyperlight-diagram.png" alt="Image" style="max-width: 100px;">
 
 [1] [Non-Proportional Parametrizations for Stable Hypernetwork Learning](https://arxiv.org/abs/2304.07645)
 
 ## Installation
 
-HyperLight can be installed via `pip`. For the **stable** version:
+To install the **stable** version of HyperLight via `pip`:
 
 ```shell
 pip install hyperlight
 ```
 
 Or for the **latest** version:
 
 ```shell
 pip install git+https://github.com/JJGO/hyperlight.git
 ```
 
-You can also **manually** install it by cloning it, installing dependencias and adding it to your `PYTHONPATH`:
+For the **manual** install:
 
 
 ```shell
+# clone it
 git clone https://github.com/JJGO/hyperlight
+
+# install dependencies
 python -m pip install -r ./hyperlight/requirements.txt # only dependency is PyTorch
 
-# Put this on your .bashrc/.zshrc
+# add this to your .bashrc/.zshrc
 export PYTHONPATH="$PYTHONPATH:/path/to/hyperlight)"
 ```
 
 
 ## Getting Started
 
 The main advantage of HyperLight is that it allows to easily reuse existing networks without having to redo the model code.
 
-For example, here's how we can write a Bayesian Neural Hypernetwork for the resnet18 architecture.
+For example, here's a Bayesian Neural Hypernetwork for the resnet18 architecture:
 
 ```python
 from torchvision.models import resnet18
-from hyperlight import hypernetize, Hypernet, find_modules_of_type
+import hyperlight as hl
 
-# First we instantiate the main network and
+# First, instantiate the main network and
 # hyperparametrize all convolutional weights
 mainnet = resnet18()
-modules = find_modules_of_type(mainnet, [nn.Conv2d])
+modules = hl.find_modules_of_type(mainnet, [nn.Conv2d])
 
 # Replace nn.Parameter objects with ExternalParameters
-mainnet = hypernetize(mainnet, modules=modules)
+mainnet = hl.hypernetize(mainnet, modules=modules)
 
-# Now, we get the spec of the weights we need to predict
+# Get the spec of the weights we need to predict
 parameter_shapes = mainnet.external_shapes()
 
 # We can predict these shapes any way we want,
 # but hyperlight provides hypernetwork models
 hyperparam_shape = {'h': (10,)} # 10-dim input
-hypernet = Hypernet(
+hypernet = hl.Hypernet(
     input_shapes=hyperparam_shape,
     output_shapes=parameter_shapes,
     hidden_sizes=[16,64,128],
 )
 
 # Now, instead of model(input) we first predict the main network weights
-parameters = hypernet(h=hyperpameter_input)
+parameters = hl.hypernet(h=hyperpameter_input)
 
 # and then use the main network
 with mainnet.using_externals(parameters):
-    # within this context manager, the weights are accesible
+    # Within this context manager, the weights are accessible
     prediction = mainnet(input)
 
-    # after this point, weights are removed
+    # After this point, weights are removed
 ```
 
-We can also wrap this into `nn.Module` to pair-up the hypernet with the main network and have a nicer API
+We can also wrap this into `nn.Module` to pair-up the hypernet with the main network and have a nicer API:
 
 ```python
 
 class HyperResNet18(nn.Module):
 
     def __init__(self,
         hypernet_layers: List[]
         ):
         super().__init__()
         mainnet = resnet18()
-        modules = find_modules_of_type(mainnet, [nn.Conv2d])
-        mainnet = hypernetize(mainnet, modules=modules)
+        modules = hl.find_modules_of_type(mainnet, [nn.Conv2d])
+        self.mainnet = hl.hypernetize(mainnet, modules=modules)
 
-        hypernet = Hypernet(
+        self.hypernet = hl.Hypernet(
             input_shapes={'h': (10,)},
             output_shapes=parameter_shapes,
             layer_sizes=[16,64,128],
         )
 
     def forward(self, input, hyper_input):
-        parameters = hypernet(h=hyper_input)
+        parameters = self.hypernet(h=hyper_input)
 
-        with mainnet.using_externals(parameters):
-            prediction = mainnet(input)
+        with self.mainnet.using_externals(parameters):
+            prediction = self.mainnet(input)
 
         return input
 ```
 
 
-HyperLight let us reuse the pretrained weights by setting them as independent weights
+With HyperLight, we can reuse the pretrained weights by setting them as independent weights:
 
 
 ```python
 
 class HyperResNet18(nn.Module):
 
     def __init__(self,
         hypernet_layers: List[]
         ):
         super().__init__()
         # Load pretrained weights
         mainnet = resnet18(pretrained=True)
-        modules = find_modules_of_type(mainnet, [nn.Conv2d])
-        mainnet, weights = hypernetize(mainnet, modules=modules, return_values=True)
+        modules = hl.find_modules_of_type(mainnet, [nn.Conv2d])
+        self.mainnet, weights = hl.hypernetize(mainnet, modules=modules, return_values=True)
 
         # Construct from existing
-        hypernet = Hypernet.from_existing(
-            weights, # The weights encode shape and intialization
+        self.hypernet = hl.Hypernet.from_existing(
+            weights, # weights encode shape and initialization
             input_shapes={'h': (10,)},
             output_shapes=parameter_shapes,
             layer_sizes=[16,64,128],
         )
 
     def forward(self, input, hyper_input):
-        parameters = hypernet(h=hyper_input)
+        parameters = self.hypernet(h=hyper_input)
 
-        with mainnet.using_externals(parameters):
-            prediction = mainnet(input)
+        with self.mainnet.using_externals(parameters):
+            prediction = self.mainnet(input)
 
         return input
 ```
 
 ## Tutorial
 
 ### Concepts
 
-In Hyperlight there are a few new concepts:
+HyperLight introduces a few new concepts:
 
-- `HyperModule` - Specialized `nn.Module` objects that can hold both regular parameters
-and `ExternalParameters` to be predicted by a external hypernetwork.
-- `ExternalParameter` - `nn.Parameter` replacements that only stores the required shape of the
+- `HyperModule` – A specialized `nn.Module` object that can hold both regular parameters
+and `ExternalParameters` to be predicted by an external hypernetwork.
+- `ExternalParameter` – `nn.Parameter` replacement that only stores the required shape of the
 externalized parameter. Parameter data can be set and reset with the hypernetwork predictions.
-- `HyperNetwork` - `nn.Module` that predicts a main network parameters for a given input
+- `HyperNetwork` – `nn.Module` that predicts a main network parameters for a given input.
 
 ### Defining a `HyperModule` with `ExternalParameter`s
 
-Here is an example of how we can define a hypernetized Linear layer. We need to make sure to
-define the `ExternalParameter` properties with their correct shapes
+Here is an example of how we define a hypernetized Linear layer. We need to make sure to
+define the `ExternalParameter` properties with their correct shapes.
 
 ```python
 import torch.nn.functional as F
-from hyperlight import HyperModule, ExternalParameter
+import hyperlight as hl
 
-class HyperLinear(HyperModule):
-    """Layer that implements a nn.Linear layer but with external parameters
-    that will be predicted by a external hypernetwork"""
+class HyperLinear(hl.HyperModule):
+    """Implementation of a nn.Linear layer but with external parameters
+    that will be predicted by an external hypernetwork"""
 
     in_features: int
     out_features: int
 
     def __init__(self, in_features: int, out_features: int, bias: bool = True) -> None:
         super().__init__()
         assert isinstance(in_features, int) and isinstance(out_features, int)
         self.in_features = in_features
         self.out_features = out_features
-        self.weight = ExternalParameter(shape=(out_features, in_features))
+        self.weight = hl.ExternalParameter(shape=(out_features, in_features))
         if bias:
-            self.bias = ExternalParameter(shape=(out_features,))
+            self.bias = hl.ExternalParameter(shape=(out_features,))
         else:
             self.bias = None
 
     def forward(self, input: Tensor) -> Tensor:
         return F.linear(input, self.weight, self.bias)
 ```
 
-Once defined, we can make use of this module in the following way
+Once defined, we can make use of this module as follows:
 
 
 ```python
 >>> layer = HyperLinear(in_features=8, out_features=16)
 >>> layer.external_shapes()
 {'weight': (16, 8), 'bias': (16,)}
 >>> x = torch.zeros(1, 8)
 
-# Layer cannot be used until weights are set
+# We need to set the weights before using the layer
 >>> layer(x)
 [...]
 AttributeError: Uninitialized External Parameter, please set the value first
 
-# We need to set the external weights first
+# Initialize the external weights
 >>> layer.set_externals(weight=torch.rand(size=(16,8)), bias=torch.zeros((16,)))
 >>> layer(x).shape
 torch.Size([1, 16])
 
 # Once we are done, we reset the external parameter values
 >>> layer.reset_externals()
 ```
 
 Alternatively, we can use the `using_externals` contextmanager that will set and reset
-the parameters accordingly
+the parameters accordingly:
 
 ```python
 params(weight=torch.rand(size=(16,8)), bias=torch.zeros((16,)))
 with layer.using_externals(params):
     y = layer(x)
 ```
 
 ### Dynamically hypernetizing modules
 
 HyperLight supports **dynamic** HyperModule creation using the `hypernetize` helper.
-We need to specify what parameters we want to remove fromt the module and convert to
-`ExternalParameter` objects.
+We need to specify which parameters we want to remove from the module and convert to
+`ExternalParameter` objects:
 
 ```python
 >>> from torch import nn
->>> from hyperlight import hypernetize, hypernetize_single
+>>> import hyperlight as hl
 
 >>> layer = nn.Linear(in_features=8, out_features=16)
->>> layer = hypernetize(layer, parameters=[layer.weight, layer.bias])
+>>> layer = hl.hypernetize(layer, parameters=[layer.weight, layer.bias])
 >>> layer
 HypernetizedLinear()
 >>> layer.external_shapes()
 {'weight': (16, 8), 'bias': (16,)}
 ```
 
-`hypernetize` is recursive, and supports entire modules being specified
+`hypernetize` is recursive, and supports entire modules being specified:
 
 
 ```python
 >>> model = nn.Sequential(OrderedDict({
     'conv': nn.Conv2d(3,128,3),
     'norm': nn.BatchNorm2d(128),
     'relu': nn.ReLU(),
     'pool': nn.AdaptiveAvgPool2d((1,1)),
     'out': nn.Linear(128, 10)
 }))
 
->>> model = hypernetize(model, modules=[model.conv, model.out])
+>>> model = hl.hypernetize(model, modules=[model.conv, model.out])
 >>>  model.external_shapes()
 {'conv.weight': (128, 3, 3, 3),
  'conv.bias': (128,),
  'out.weight': (10, 128),
  'out.bias': (10,)}
 ```
 
 ### Finding modules and parameters
 
-Additionally, Hyperlight provides several routines to recursively search for parameters and modules to feed
-into `hypernetize`:
+In addition, HyperLight provides several routines to recursively search for parameters and modules to feed into `hypernetize`:
 
-- `find_modules_of_type(model, module_types)` – To find modules from a certain type,
+- `find_modules_of_type(model, module_types)` – Find modules of a certain type,
 e.g. `nn.Linear` or `nn.Conv2d`
-- `find_modules_from_patterns(model, globs=None, regex=None)` – To find modules matching
-specific patterns usingglobs, e.g. `*.conv`; or regexes `e.g. layer[1-3].*conv`
-- `find_parameters_from_patterns(model, globs=None, regex=None)` – To find parameter
-matching specific patterns.
+- `find_modules_from_patterns(model, globs=None, regex=None)` – Find modules that match
+specific patterns using globs, e.g. `*.conv`; or regexes, e.g. `layer[1-3].*conv`
+- `find_parameters_from_patterns(model, globs=None, regex=None)` – Find parameters
+that match specific patterns.
 
 Some examples on a ResNet18 architecture:
 
 ```python
 >>> from torchvision.models import resnet18
->>> from hyperlight import find_modules_of_type
+>>> import hyperlight as hl
 >>> model = resnet18()
-# All convolutions
->>> find_modules_of_type(model, [nn.Conv2d])
+
+# Find all convolutions
+>>> hl.find_modules_of_type(model, [nn.Conv2d])
 {'conv1': Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False),
  'layer1.0.conv1': Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False),
  'layer1.0.conv2': Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False),
  ...
 
-# First convolution of every ResNet block
->>> find_modules_from_patterns(model, regex=['^layer\d.0.conv1'])
+# Find the first convolution of each ResNet block
+>>> hl.find_modules_from_patterns(model, regex=['^layer\d.0.conv1'])
 {'layer1.0.conv1': Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False),
  'layer2.0.conv1': Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False),
  'layer3.0.conv1': Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False),
  'layer4.0.conv1': Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)}
 
-# Getting just the convolutional weights of the first block (no biases)
->>> find_parameters_from_patterns(model, globs=['layer1*conv*.weight']).keys()
+# Get only the convolutional weights of the first block (no biases)
+>>> hl.find_parameters_from_patterns(model, globs=['layer1*conv*.weight']).keys()
 dict_keys(['layer1.0.conv2.weight', 'layer1.0.conv1.weight', 'layer1.1.conv1.weight', 'layer1.1.conv2.weight'])
 ```
 
+### Other methods
+
+HyperLight goes beyond hypernetworks and helps implement other Deep Learning techniques related to hypernetworks.
+
+As an example, the following code implements [FiLM](https://arxiv.org/pdf/1709.07871.pdf). Instead of having to modify
+our entire forward pass to keep track of the $\gamma$ and $\beta$ coefficients, we can have HyperLight handle that for us:
+
+
+```python
+
+import hyperlight as hl
+
+class FiLM(hl.HyperModule):
+
+    def __init__(self,
+        n_features: int
+    ):
+        super().__init__()
+        self.n_features = n_features
+        self.gamma = hl.ExternalParameter((n_features,))
+        self.beta = hl.ExternalParameter((n_features,))
+
+    def forward(self, x):
+        return self.gamma * x + self.beta
+
+
+class CNNwithFiLM(hl.HyperModule):
+    def __init__(self):
+        super().__init__()
+        self.layers = nn.Sequential([
+            nn.Conv2d(3,64,kernel_size=3,padding=1),
+            FiLM(64),
+            nn.LeakyReLU(),
+            nn.BatchNorm2d(64)
+            nn.Conv2d(64,128,kernel_size=3,padding=1),
+            FiLM(128),
+            nn.LeakyReLU(),
+            nn.BatchNorm2d(128)
+            nn.Conv2d(128,256,kernel_size=3,padding=1),
+            FiLM(256),
+            nn.LeakyReLU(),
+            nn.BatchNorm2d(256)
+            nn.AdaptiveAvgPool2d((1,1)),
+        ])
+
+def FiLM_Model(nn.Module):
+    def __init__(self, embedding_size):
+        self.main = CNNwithFiLM()
+        self.aux = hl.Hypernet(
+            input_shapes={'film_input': (embedding_size,)},
+            output_shapes=self.main.external_shapes(),
+            hidden_sizes=[],
+        )
+
+    def forward(self, input, conditioning):
+        params = self.aux(film_input=conditioning)
+        with self.main.using_externals(params):
+            return self.main(input)
+```
+
 
 ## Citation
 
 If you find our work or any of our materials useful, please cite our paper:
 
 ```
 @article{ortiz2023nonproportional,
```

### Comparing `hyperlight-0.0.3/hyperlight/convert.py` & `hyperlight-0.0.4/hyperlight/convert.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/hyperlight/find.py` & `hyperlight-0.0.4/hyperlight/find.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/hyperlight/hypernet/encoding.py` & `hyperlight-0.0.4/hyperlight/hypernet/encoding.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/hyperlight/hypernet/initialization.py` & `hyperlight-0.0.4/hyperlight/hypernet/initialization.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/hyperlight/hypernet/model.py` & `hyperlight-0.0.4/hyperlight/hypernet/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         init_distribution: Optional[str] = "kaiming_normal_fanout",
         init_bias: Optional[float] = 0.0,
     ) -> None:
         """
         Creates a fully connected neural network with specified input size, hidden sizes,
         output size, dropout probability and activation function.
 
+        The default choice of 'fan out' init is done on purpose as hypernetworks tend to
+        substantially increase the number of neurons, specially in the last layer
+
         Args:
             input_size (int): Dimension of input
             hidden_sizes (List[int]): List of hidden layer dimensions
             output_size (int): Dimension of output
             dropout_prob (float): Dropout probability (default=0)
             nonlinearity (str): Nonlinear activation function (default='LeakyReLU')
             out_bias (bool): Whether last layer should have bias (default=True)
@@ -237,22 +240,34 @@
                 shape = (batch_dim, *shape)
             outputs[name] = flat_output.narrow(1, *self._output_offsets[name]).view(
                 shape
             )
         return outputs
 
 
-class HyperNet(nn.Module, HyperNetMixin):
+class HyperNet(nn.Module):
+    """A hypernetwork that generates weights for a target network. Shape is Dict[str, Tuple[int, ...]]
+
+    Args:
+        input_shapes (Dict[str, Shape]): The shapes of the inputs that the hypernetwork takes
+        output_shapes (Dict[str, Shape]): The shapes of the primary network weights being predicted,
+        hidden_sizes (List[int]): The sizes of the hidden layers of the hypernetwork.
+        encoding (InputMode, optional): The input encoding mode. Defaults to "cos|sin".
+        init_independent_weights (bool, optional): Whether to init weights independently. Defaults to True.
+        output_split_init (bool, optional): Whether to initialize the output split. Defaults to True.
+        fc_kws (Dict[str, Any], optional): Keyword arguments for the fully connected layers. Defaults to None.
+    """
     def __init__(
         self,
         input_shapes: Dict[str, Shape],
         output_shapes: Dict[str, Shape],
         hidden_sizes: List[int],
         encoding: InputMode = "cos|sin",
         init_independent_weights: bool = True,
+        output_split_init: bool = True,
         fc_kws: Optional[Dict[str, Any]] = None,
     ):
         super().__init__()
 
         if not isinstance(input_shapes, dict):
             input_shapes = dict(input_shapes)
         if not isinstance(output_shapes, dict):
@@ -272,14 +287,42 @@
             output_size=self.flat_output_size(),
             **(fc_kws or {}),
         )
 
         if init_independent_weights:
             self.init_independent_weights()
 
+        if output_split_init:
+            self._init_output_split()
+
+    def _init_output_split(self):
+        """
+        Helper function that initializes the MLP last fully connected layer
+        as N independent layers. This is important because the fan_out scheme
+        will substantially change depending on the number of predicted neurons
+
+        Moreover, if the layer is predicting a bias, we initialize it to zero
+        """
+
+        output_weight = self.backbone.output.weight
+        nonlinearity = self.backbone.nonlinearity
+        init_distribution = self.backbone.init_distribution
+
+        for name in self.output_shapes:
+            offset, length = self._output_offsets[name]
+            tensor = output_weight[offset:offset+length,:]
+            if name.endswith('.bias'):
+                # Bias should initialize to zero
+                initialize_weight(tensor, 'zeros')
+            elif name.endswith('.weight'):
+                initialize_weight(tensor, init_distribution, nonlinearity=nonlinearity)
+            else:
+                initialize_weight(tensor, init_distribution, nonlinearity=nonlinearity)
+
+
     @classmethod
     def from_existing(cls, weights: Dict[str, Tensor], **kwargs) -> "HyperNet":
         output_shapes = {k: v.shape for k, v in weights.items()}
         hypernet = cls(output_shapes=output_shapes, **kwargs)
         hypernet.set_independent_weights(weights)
         return hypernet
```

### Comparing `hyperlight-0.0.3/hyperlight/nn/container.py` & `hyperlight-0.0.4/hyperlight/nn/container.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/hyperlight/nn/layers.py` & `hyperlight-0.0.4/hyperlight/nn/layers.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/hyperlight/nn/module.py` & `hyperlight-0.0.4/hyperlight/nn/module.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/hyperlight/nn/xparam.py` & `hyperlight-0.0.4/hyperlight/nn/xparam.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.3/pyproject.toml` & `hyperlight-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hyperlight"
 homepage = "https://github.com/JJGO/hyperlight"
 documentation = "https://github.com/JJGO/hyperlight"
-version = "0.0.3"
+version = "0.0.4"
 description = "Hyperlight is a Pytorch hypernetwork framework with a streamlined API"
 authors = ["Jose Javier Gonzalez Ortiz <josejg@mit.edu>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers=[
     'Intended Audience :: Science/Research',
     'Intended Audience :: Developers',
@@ -35,15 +35,15 @@
 pyright = "^1.2.0"
 pre-commit = "^2.17.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `hyperlight-0.0.3/PKG-INFO` & `hyperlight-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperlight
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hyperlight is a Pytorch hypernetwork framework with a streamlined API
 Home-page: https://github.com/JJGO/hyperlight
 License: Apache-2.0
 Keywords: hyperlight,pytorch,hypernetworks,deep learning
 Author: Jose Javier Gonzalez Ortiz
 Author-email: josejg@mit.edu
 Requires-Python: >=3.7,<4.0
@@ -23,316 +23,382 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: torch (>=1.10,<3)
 Project-URL: Documentation, https://github.com/JJGO/hyperlight
 Description-Content-Type: text/markdown
 
 # HyperLight
 
-> Hypernetworks in Pytorch made easy
+_Hypernetworks in Pytorch made easy_
 
 [![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat&amp;logo=PyTorch&amp;logoColor=white)](https://pytorch.org)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/hyperlight)](https://pypi.org/project/hyperlight/) 
 [![PyPI version](https://badge.fury.io/py/hyperlight.svg)](https://badge.fury.io/py/hyperlight)
 [![Downloads](https://pepy.tech/badge/hyperlight)](https://pepy.tech/project/hyperlight)
 [![license](https://img.shields.io/github/license/JJGO/hyperlight.svg)](https://github.com/JJGO/hyperlight/blob/main/LICENSE)
 
+
 ## TL;DR
 
 HyperLight is a Pytorch library designed to make implementing hypernetwork models easy and painless.
 What sets HyperLight apart from other hypernetwork implementations:
 
-- **Bring your own architecture** – HyperLight lets you reuse your existing model code.
+- **Bring your own architecture** – Reuse your existing model code.
 - **Principled Parametrizations and Initializations** – Default networks can have unstable training dynamics, HyperLight has good defaults that lead to improved training [1].
-- **Work with pretrained models** – Pretrained weights can be used as part of the hypernetwork initialization.
-- **Seemless Composability** – It's hypernets all the way down! You can hypernetize hypernet models without issue.
-- **_Pytorch-nic_ API design** – Parameters are not treated as inputs to layers, preventing lots of code rewriting from happening.
+- **Work with pretrained models** – Use pretrained weights as part of the hypernetwork initialization.
+- **Seamless Composability** – It's hypernets all the way down! Hypernetize hypernet models without issue.
+- **_Pytorch-nic_ API design** – Parameters are treated as an attribute of the layer, preventing the need for rewriting PyTorch modules.
 <!-- - **Easy weight reuse** – Once a model has its weights set, it can be used many times. -->
+<br>
+<img src="https://raw.githubusercontent.com/JJGO/hyperlight/assets/hyperlight-diagram.png" alt="Image" style="max-width: 100px;">
 
 [1] [Non-Proportional Parametrizations for Stable Hypernetwork Learning](https://arxiv.org/abs/2304.07645)
 
 ## Installation
 
-HyperLight can be installed via `pip`. For the **stable** version:
+To install the **stable** version of HyperLight via `pip`:
 
 ```shell
 pip install hyperlight
 ```
 
 Or for the **latest** version:
 
 ```shell
 pip install git+https://github.com/JJGO/hyperlight.git
 ```
 
-You can also **manually** install it by cloning it, installing dependencias and adding it to your `PYTHONPATH`:
+For the **manual** install:
 
 
 ```shell
+# clone it
 git clone https://github.com/JJGO/hyperlight
+
+# install dependencies
 python -m pip install -r ./hyperlight/requirements.txt # only dependency is PyTorch
 
-# Put this on your .bashrc/.zshrc
+# add this to your .bashrc/.zshrc
 export PYTHONPATH="$PYTHONPATH:/path/to/hyperlight)"
 ```
 
 
 ## Getting Started
 
 The main advantage of HyperLight is that it allows to easily reuse existing networks without having to redo the model code.
 
-For example, here's how we can write a Bayesian Neural Hypernetwork for the resnet18 architecture.
+For example, here's a Bayesian Neural Hypernetwork for the resnet18 architecture:
 
 ```python
 from torchvision.models import resnet18
-from hyperlight import hypernetize, Hypernet, find_modules_of_type
+import hyperlight as hl
 
-# First we instantiate the main network and
+# First, instantiate the main network and
 # hyperparametrize all convolutional weights
 mainnet = resnet18()
-modules = find_modules_of_type(mainnet, [nn.Conv2d])
+modules = hl.find_modules_of_type(mainnet, [nn.Conv2d])
 
 # Replace nn.Parameter objects with ExternalParameters
-mainnet = hypernetize(mainnet, modules=modules)
+mainnet = hl.hypernetize(mainnet, modules=modules)
 
-# Now, we get the spec of the weights we need to predict
+# Get the spec of the weights we need to predict
 parameter_shapes = mainnet.external_shapes()
 
 # We can predict these shapes any way we want,
 # but hyperlight provides hypernetwork models
 hyperparam_shape = {'h': (10,)} # 10-dim input
-hypernet = Hypernet(
+hypernet = hl.Hypernet(
     input_shapes=hyperparam_shape,
     output_shapes=parameter_shapes,
     hidden_sizes=[16,64,128],
 )
 
 # Now, instead of model(input) we first predict the main network weights
-parameters = hypernet(h=hyperpameter_input)
+parameters = hl.hypernet(h=hyperpameter_input)
 
 # and then use the main network
 with mainnet.using_externals(parameters):
-    # within this context manager, the weights are accesible
+    # Within this context manager, the weights are accessible
     prediction = mainnet(input)
 
-    # after this point, weights are removed
+    # After this point, weights are removed
 ```
 
-We can also wrap this into `nn.Module` to pair-up the hypernet with the main network and have a nicer API
+We can also wrap this into `nn.Module` to pair-up the hypernet with the main network and have a nicer API:
 
 ```python
 
 class HyperResNet18(nn.Module):
 
     def __init__(self,
         hypernet_layers: List[]
         ):
         super().__init__()
         mainnet = resnet18()
-        modules = find_modules_of_type(mainnet, [nn.Conv2d])
-        mainnet = hypernetize(mainnet, modules=modules)
+        modules = hl.find_modules_of_type(mainnet, [nn.Conv2d])
+        self.mainnet = hl.hypernetize(mainnet, modules=modules)
 
-        hypernet = Hypernet(
+        self.hypernet = hl.Hypernet(
             input_shapes={'h': (10,)},
             output_shapes=parameter_shapes,
             layer_sizes=[16,64,128],
         )
 
     def forward(self, input, hyper_input):
-        parameters = hypernet(h=hyper_input)
+        parameters = self.hypernet(h=hyper_input)
 
-        with mainnet.using_externals(parameters):
-            prediction = mainnet(input)
+        with self.mainnet.using_externals(parameters):
+            prediction = self.mainnet(input)
 
         return input
 ```
 
 
-HyperLight let us reuse the pretrained weights by setting them as independent weights
+With HyperLight, we can reuse the pretrained weights by setting them as independent weights:
 
 
 ```python
 
 class HyperResNet18(nn.Module):
 
     def __init__(self,
         hypernet_layers: List[]
         ):
         super().__init__()
         # Load pretrained weights
         mainnet = resnet18(pretrained=True)
-        modules = find_modules_of_type(mainnet, [nn.Conv2d])
-        mainnet, weights = hypernetize(mainnet, modules=modules, return_values=True)
+        modules = hl.find_modules_of_type(mainnet, [nn.Conv2d])
+        self.mainnet, weights = hl.hypernetize(mainnet, modules=modules, return_values=True)
 
         # Construct from existing
-        hypernet = Hypernet.from_existing(
-            weights, # The weights encode shape and intialization
+        self.hypernet = hl.Hypernet.from_existing(
+            weights, # weights encode shape and initialization
             input_shapes={'h': (10,)},
             output_shapes=parameter_shapes,
             layer_sizes=[16,64,128],
         )
 
     def forward(self, input, hyper_input):
-        parameters = hypernet(h=hyper_input)
+        parameters = self.hypernet(h=hyper_input)
 
-        with mainnet.using_externals(parameters):
-            prediction = mainnet(input)
+        with self.mainnet.using_externals(parameters):
+            prediction = self.mainnet(input)
 
         return input
 ```
 
 ## Tutorial
 
 ### Concepts
 
-In Hyperlight there are a few new concepts:
+HyperLight introduces a few new concepts:
 
-- `HyperModule` - Specialized `nn.Module` objects that can hold both regular parameters
-and `ExternalParameters` to be predicted by a external hypernetwork.
-- `ExternalParameter` - `nn.Parameter` replacements that only stores the required shape of the
+- `HyperModule` – A specialized `nn.Module` object that can hold both regular parameters
+and `ExternalParameters` to be predicted by an external hypernetwork.
+- `ExternalParameter` – `nn.Parameter` replacement that only stores the required shape of the
 externalized parameter. Parameter data can be set and reset with the hypernetwork predictions.
-- `HyperNetwork` - `nn.Module` that predicts a main network parameters for a given input
+- `HyperNetwork` – `nn.Module` that predicts a main network parameters for a given input.
 
 ### Defining a `HyperModule` with `ExternalParameter`s
 
-Here is an example of how we can define a hypernetized Linear layer. We need to make sure to
-define the `ExternalParameter` properties with their correct shapes
+Here is an example of how we define a hypernetized Linear layer. We need to make sure to
+define the `ExternalParameter` properties with their correct shapes.
 
 ```python
 import torch.nn.functional as F
-from hyperlight import HyperModule, ExternalParameter
+import hyperlight as hl
 
-class HyperLinear(HyperModule):
-    """Layer that implements a nn.Linear layer but with external parameters
-    that will be predicted by a external hypernetwork"""
+class HyperLinear(hl.HyperModule):
+    """Implementation of a nn.Linear layer but with external parameters
+    that will be predicted by an external hypernetwork"""
 
     in_features: int
     out_features: int
 
     def __init__(self, in_features: int, out_features: int, bias: bool = True) -> None:
         super().__init__()
         assert isinstance(in_features, int) and isinstance(out_features, int)
         self.in_features = in_features
         self.out_features = out_features
-        self.weight = ExternalParameter(shape=(out_features, in_features))
+        self.weight = hl.ExternalParameter(shape=(out_features, in_features))
         if bias:
-            self.bias = ExternalParameter(shape=(out_features,))
+            self.bias = hl.ExternalParameter(shape=(out_features,))
         else:
             self.bias = None
 
     def forward(self, input: Tensor) -> Tensor:
         return F.linear(input, self.weight, self.bias)
 ```
 
-Once defined, we can make use of this module in the following way
+Once defined, we can make use of this module as follows:
 
 
 ```python
 >>> layer = HyperLinear(in_features=8, out_features=16)
 >>> layer.external_shapes()
 {'weight': (16, 8), 'bias': (16,)}
 >>> x = torch.zeros(1, 8)
 
-# Layer cannot be used until weights are set
+# We need to set the weights before using the layer
 >>> layer(x)
 [...]
 AttributeError: Uninitialized External Parameter, please set the value first
 
-# We need to set the external weights first
+# Initialize the external weights
 >>> layer.set_externals(weight=torch.rand(size=(16,8)), bias=torch.zeros((16,)))
 >>> layer(x).shape
 torch.Size([1, 16])
 
 # Once we are done, we reset the external parameter values
 >>> layer.reset_externals()
 ```
 
 Alternatively, we can use the `using_externals` contextmanager that will set and reset
-the parameters accordingly
+the parameters accordingly:
 
 ```python
 params(weight=torch.rand(size=(16,8)), bias=torch.zeros((16,)))
 with layer.using_externals(params):
     y = layer(x)
 ```
 
 ### Dynamically hypernetizing modules
 
 HyperLight supports **dynamic** HyperModule creation using the `hypernetize` helper.
-We need to specify what parameters we want to remove fromt the module and convert to
-`ExternalParameter` objects.
+We need to specify which parameters we want to remove from the module and convert to
+`ExternalParameter` objects:
 
 ```python
 >>> from torch import nn
->>> from hyperlight import hypernetize, hypernetize_single
+>>> import hyperlight as hl
 
 >>> layer = nn.Linear(in_features=8, out_features=16)
->>> layer = hypernetize(layer, parameters=[layer.weight, layer.bias])
+>>> layer = hl.hypernetize(layer, parameters=[layer.weight, layer.bias])
 >>> layer
 HypernetizedLinear()
 >>> layer.external_shapes()
 {'weight': (16, 8), 'bias': (16,)}
 ```
 
-`hypernetize` is recursive, and supports entire modules being specified
+`hypernetize` is recursive, and supports entire modules being specified:
 
 
 ```python
 >>> model = nn.Sequential(OrderedDict({
     'conv': nn.Conv2d(3,128,3),
     'norm': nn.BatchNorm2d(128),
     'relu': nn.ReLU(),
     'pool': nn.AdaptiveAvgPool2d((1,1)),
     'out': nn.Linear(128, 10)
 }))
 
->>> model = hypernetize(model, modules=[model.conv, model.out])
+>>> model = hl.hypernetize(model, modules=[model.conv, model.out])
 >>>  model.external_shapes()
 {'conv.weight': (128, 3, 3, 3),
  'conv.bias': (128,),
  'out.weight': (10, 128),
  'out.bias': (10,)}
 ```
 
 ### Finding modules and parameters
 
-Additionally, Hyperlight provides several routines to recursively search for parameters and modules to feed
-into `hypernetize`:
+In addition, HyperLight provides several routines to recursively search for parameters and modules to feed into `hypernetize`:
 
-- `find_modules_of_type(model, module_types)` – To find modules from a certain type,
+- `find_modules_of_type(model, module_types)` – Find modules of a certain type,
 e.g. `nn.Linear` or `nn.Conv2d`
-- `find_modules_from_patterns(model, globs=None, regex=None)` – To find modules matching
-specific patterns usingglobs, e.g. `*.conv`; or regexes `e.g. layer[1-3].*conv`
-- `find_parameters_from_patterns(model, globs=None, regex=None)` – To find parameter
-matching specific patterns.
+- `find_modules_from_patterns(model, globs=None, regex=None)` – Find modules that match
+specific patterns using globs, e.g. `*.conv`; or regexes, e.g. `layer[1-3].*conv`
+- `find_parameters_from_patterns(model, globs=None, regex=None)` – Find parameters
+that match specific patterns.
 
 Some examples on a ResNet18 architecture:
 
 ```python
 >>> from torchvision.models import resnet18
->>> from hyperlight import find_modules_of_type
+>>> import hyperlight as hl
 >>> model = resnet18()
-# All convolutions
->>> find_modules_of_type(model, [nn.Conv2d])
+
+# Find all convolutions
+>>> hl.find_modules_of_type(model, [nn.Conv2d])
 {'conv1': Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False),
  'layer1.0.conv1': Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False),
  'layer1.0.conv2': Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False),
  ...
 
-# First convolution of every ResNet block
->>> find_modules_from_patterns(model, regex=['^layer\d.0.conv1'])
+# Find the first convolution of each ResNet block
+>>> hl.find_modules_from_patterns(model, regex=['^layer\d.0.conv1'])
 {'layer1.0.conv1': Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False),
  'layer2.0.conv1': Conv2d(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False),
  'layer3.0.conv1': Conv2d(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False),
  'layer4.0.conv1': Conv2d(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)}
 
-# Getting just the convolutional weights of the first block (no biases)
->>> find_parameters_from_patterns(model, globs=['layer1*conv*.weight']).keys()
+# Get only the convolutional weights of the first block (no biases)
+>>> hl.find_parameters_from_patterns(model, globs=['layer1*conv*.weight']).keys()
 dict_keys(['layer1.0.conv2.weight', 'layer1.0.conv1.weight', 'layer1.1.conv1.weight', 'layer1.1.conv2.weight'])
 ```
 
+### Other methods
+
+HyperLight goes beyond hypernetworks and helps implement other Deep Learning techniques related to hypernetworks.
+
+As an example, the following code implements [FiLM](https://arxiv.org/pdf/1709.07871.pdf). Instead of having to modify
+our entire forward pass to keep track of the $\gamma$ and $\beta$ coefficients, we can have HyperLight handle that for us:
+
+
+```python
+
+import hyperlight as hl
+
+class FiLM(hl.HyperModule):
+
+    def __init__(self,
+        n_features: int
+    ):
+        super().__init__()
+        self.n_features = n_features
+        self.gamma = hl.ExternalParameter((n_features,))
+        self.beta = hl.ExternalParameter((n_features,))
+
+    def forward(self, x):
+        return self.gamma * x + self.beta
+
+
+class CNNwithFiLM(hl.HyperModule):
+    def __init__(self):
+        super().__init__()
+        self.layers = nn.Sequential([
+            nn.Conv2d(3,64,kernel_size=3,padding=1),
+            FiLM(64),
+            nn.LeakyReLU(),
+            nn.BatchNorm2d(64)
+            nn.Conv2d(64,128,kernel_size=3,padding=1),
+            FiLM(128),
+            nn.LeakyReLU(),
+            nn.BatchNorm2d(128)
+            nn.Conv2d(128,256,kernel_size=3,padding=1),
+            FiLM(256),
+            nn.LeakyReLU(),
+            nn.BatchNorm2d(256)
+            nn.AdaptiveAvgPool2d((1,1)),
+        ])
+
+def FiLM_Model(nn.Module):
+    def __init__(self, embedding_size):
+        self.main = CNNwithFiLM()
+        self.aux = hl.Hypernet(
+            input_shapes={'film_input': (embedding_size,)},
+            output_shapes=self.main.external_shapes(),
+            hidden_sizes=[],
+        )
+
+    def forward(self, input, conditioning):
+        params = self.aux(film_input=conditioning)
+        with self.main.using_externals(params):
+            return self.main(input)
+```
+
 
 ## Citation
 
 If you find our work or any of our materials useful, please cite our paper:
 
 ```
 @article{ortiz2023nonproportional,
```

