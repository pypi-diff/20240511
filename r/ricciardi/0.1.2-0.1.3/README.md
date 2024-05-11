# Comparing `tmp/ricciardi-0.1.2.tar.gz` & `tmp/ricciardi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricciardi-0.1.2.tar", last modified: Thu Apr 25 22:35:44 2024, max compression
+gzip compressed data, was "ricciardi-0.1.3.tar", last modified: Fri May 10 20:51:59 2024, max compression
```

## Comparing `ricciardi-0.1.2.tar` & `ricciardi-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.491787 ricciardi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 22:35:40.000000 ricciardi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-25 22:35:44.491787 ricciardi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-25 22:35:40.000000 ricciardi-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-25 22:35:40.000000 ricciardi-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:35:44.491787 ricciardi-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.487787 ricciardi-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.487787 ricciardi-0.1.2/src/ricciardi/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 22:35:40.000000 ricciardi-0.1.2/src/ricciardi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-25 22:35:40.000000 ricciardi-0.1.2/src/ricciardi/ricciardi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.491787 ricciardi-0.1.2/src/ricciardi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 22:35:44.000000 ricciardi-0.1.2/src/ricciardi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:35:44.491787 ricciardi-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 22:35:40.000000 ricciardi-0.1.2/test/test_ricciardi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:51:59.832203 ricciardi-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 20:51:55.000000 ricciardi-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-10 20:51:59.832203 ricciardi-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-10 20:51:55.000000 ricciardi-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-10 20:51:55.000000 ricciardi-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:51:59.832203 ricciardi-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:51:59.828203 ricciardi-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:51:59.832203 ricciardi-0.1.3/src/ricciardi/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 20:51:55.000000 ricciardi-0.1.3/src/ricciardi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-10 20:51:55.000000 ricciardi-0.1.3/src/ricciardi/ricciardi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:51:59.832203 ricciardi-0.1.3/src/ricciardi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-10 20:51:59.000000 ricciardi-0.1.3/src/ricciardi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 20:51:59.000000 ricciardi-0.1.3/src/ricciardi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:51:59.000000 ricciardi-0.1.3/src/ricciardi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 20:51:59.000000 ricciardi-0.1.3/src/ricciardi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 20:51:59.000000 ricciardi-0.1.3/src/ricciardi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:51:59.832203 ricciardi-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-10 20:51:55.000000 ricciardi-0.1.3/test/test_ricciardi.py
```

### Comparing `ricciardi-0.1.2/LICENSE` & `ricciardi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ricciardi-0.1.2/PKG-INFO` & `ricciardi-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricciardi
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyTorch implementation of the Ricciardi transfer function.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,27 +25,34 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/hchau630/ricciardi
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: torch
 
+![tests workflow status](https://github.com/hchau630/ricciardi/actions/workflows/tests.yml/badge.svg)
+
 # About
 An efficient, GPU-friendly, and differentiable PyTorch implementation of the Ricciardi transfer function based on equations and default parameters from [Sanzeni et al. (2020)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008165).
 
 # Usage
 For using the ricciardi function in your own code, you can either just copy the source file at `src/ricciardi/ricciardi.py` to your own code, or install the package in your python environment with `pip install ricciardi` and import the function with `from ricciardi import ricciardi`. To run tests, clone the repository, create a new environment, install the neccessary packages with `pip install -r requirements`, and run the command `pytest`.
 
 # Benchmark
-Compare performance with an interpolation-based approach. Forward pass is slightly slower, but backward pass is >2x faster on GPU.
+Compare performance with a naive, linear interpolation-based approach. Forward pass is slightly slower, but backward pass is >2x faster on GPU.
 
 Results on CPU (AMD EPYC 7662, 8 cores) (`python benchmark/benchmark.py -N 100000 -r 100`):
 ```
 forward pass, requires_grad=False
 ricciardi: median=1.86 ms, min=1.84 ms (100 repeats)
 ricciardi_interp: median=1.75 ms, min=1.72 ms (100 repeats)
```

### Comparing `ricciardi-0.1.2/README.md` & `ricciardi-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+![tests workflow status](https://github.com/hchau630/ricciardi/actions/workflows/tests.yml/badge.svg)
+
 # About
 An efficient, GPU-friendly, and differentiable PyTorch implementation of the Ricciardi transfer function based on equations and default parameters from [Sanzeni et al. (2020)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008165).
 
 # Usage
 For using the ricciardi function in your own code, you can either just copy the source file at `src/ricciardi/ricciardi.py` to your own code, or install the package in your python environment with `pip install ricciardi` and import the function with `from ricciardi import ricciardi`. To run tests, clone the repository, create a new environment, install the neccessary packages with `pip install -r requirements`, and run the command `pytest`.
 
 # Benchmark
-Compare performance with an interpolation-based approach. Forward pass is slightly slower, but backward pass is >2x faster on GPU.
+Compare performance with a naive, linear interpolation-based approach. Forward pass is slightly slower, but backward pass is >2x faster on GPU.
 
 Results on CPU (AMD EPYC 7662, 8 cores) (`python benchmark/benchmark.py -N 100000 -r 100`):
 ```
 forward pass, requires_grad=False
 ricciardi: median=1.86 ms, min=1.84 ms (100 repeats)
 ricciardi_interp: median=1.75 ms, min=1.72 ms (100 repeats)
```

### Comparing `ricciardi-0.1.2/pyproject.toml` & `ricciardi-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [build-system]
 requires = ["setuptools>=64.0"]  # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ricciardi"
-version = "0.1.2"
+version = "0.1.3"
 description = "PyTorch implementation of the Ricciardi transfer function."
+requires-python = ">= 3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "scipy",
     "torch",
 ]
 
 [project.urls]
```

### Comparing `ricciardi-0.1.2/src/ricciardi/ricciardi.py` & `ricciardi-0.1.3/src/ricciardi/ricciardi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+from collections.abc import Callable
+from typing import Union
+
 import torch
+from torch import Tensor
 from scipy import special
 
 sqrtpi = torch.pi**0.5
 
 
 def _cached_roots_legendre(n):
     """
@@ -15,26 +19,33 @@
     _cached_roots_legendre.cache[n] = special.roots_legendre(n)
     return _cached_roots_legendre.cache[n]
 
 
 _cached_roots_legendre.cache = dict()
 
 
-def fixed_quad(func, a, b, args=(), n=5):
+def fixed_quad(
+    func: Callable[[Tensor], Tensor],
+    a: Tensor,
+    b: Union[float, Tensor],
+    args: tuple = (),
+    n: int = 5,
+) -> tuple[Tensor, None]:
     """Like scipy.integrate.fixed_quad, but for tensor inputs a, b
 
     Args:
-        func (Callable[[torch.Tensor, ...], torch.Tensor]): Integrand.
-        a: (torch.Tensor): Lower limits of integral.
-        b: (float | torch.Tensor): Upper limit(s) of integral.
-        args (tuple, optional): Additional arguments passed to func.
-        n (int, optional): Order of Gauss-Legendre quadrature.
+        func: Integrand.
+        a: Lower limits of integral.
+        b: Upper limit(s) of integral.
+        args (optional): Additional arguments passed to func.
+        n (optional): Order of Gauss-Legendre quadrature.
 
     Returns:
-        torch.Tensor: Tensor with shape func(broadcast(a, b)).shape
+        A tuple (value, None), where value is a tensor with shape func(broadcast(a, b)).shape.
+        The additional None is for consistency with scipy.integrate.fixed_quad.
 
     """
     x, w = _cached_roots_legendre(n)
     x = x.real
 
     d = (b - a) / 2.0
     return d * sum(wi * func(d * (xi + 1) + a, *args) for xi, wi in zip(x, w)), None
@@ -55,57 +66,71 @@
         return (
             -torch.special.erfcx(x) * grad_output,
             torch.special.erfcx(y) * grad_output,
             None,
         )
 
 
-def ierfcx(x, y, n=5):
+def ierfcx(x: Tensor, y: Union[float, Tensor], n: int = 5) -> Tensor:
     """Integral of erfcx(t) from x to y using Gauss-Legendre quadrature of order n.
 
     Args:
-        x (torch.Tensor): Lower limits of integral.
-        y (float | torch.Tensor): Upper limit(s) of integral.
-        n (int, optional): Order of Gauss-Legendre quadrature.
+        x: Lower limits of integral.
+        y: Upper limit(s) of integral.
+        n (optional): Order of Gauss-Legendre quadrature.
 
     Returns:
-        torch.Tensor: Tensor with shape broadcast(x, y).shape
+        Tensor with shape broadcast(x, y).shape
 
     """
     return Ierfcx.apply(x, y, n)
 
 
-def ricciardi(mu, sigma=0.01, tau=0.02, tau_rp=0.002, V_r=0.01, theta=0.02, n=None):
+def ricciardi(
+    mu: Tensor,
+    sigma: Union[float, Tensor] = 0.01,
+    tau: Union[float, Tensor] = 0.02,
+    tau_rp: Union[float, Tensor] = 0.002,
+    V_r: Union[float, Tensor] = 0.01,
+    theta: Union[float, Tensor] = 0.02,
+    n: Union[int, None] = None,
+) -> Tensor:
     """Ricciardi transfer function.
 
     Computes the firing rate of an LIF neuron as a function of the mean and variance
     of the presynaptic input current, with default values and notation following
     Sanzeni et al. (2020). Default values assume SI units (i.e. seconds and volts).
 
     Args:
-        mu (torch.Tensor): Mean of presynaptic input current.
-        sigma (float | torch.Tensor, optional): Standard deviation of presynaptic input current.
-        tau (float | torch.Tensor, optional): Time constant of the membrane potential.
-        tau_rp (float | torch.Tensor, optional): Refractory period.
-        V_r (float | torch.Tensor, optional): Reset membrane potential.
-        theta (float | torch.Tensor, optional): Firing threshold membrane potential.
-        n (int, optional):
-            Precision level, roughly equivalent to the order of Gauss-Legendre quadrature used to compute
-            the integral of the complementary error function. If None, defaults to 4, 5, or 6 for
-            input dtypes torch.half, torch.float, and torch.double, respectively.
+        mu: Mean of presynaptic input current.
+        sigma (optional): Standard deviation of presynaptic input current.
+        tau (optional): Time constant of the membrane potential.
+        tau_rp (optional): Refractory period.
+        V_r (optional): Reset membrane potential.
+        theta (optional): Firing threshold membrane potential.
+        n (optional): Precision level, roughly equivalent to the order of Gauss-Legendre
+          quadrature used to compute the integral of the complementary error function.
+          If None, defaults to 3, 4, 5, or 6 for input dtypes torch.bfloat16, torch.half,
+          torch.float, and torch.double, respectively.
 
     Returns:
-        torch.Tensor: Tensor of firing rates with shape broadcast(mu, sigma, tau, tau_rp, V_r, theta).shape
+        Tensor of firing rates with shape broadcast(mu, sigma, tau, tau_rp, V_r, theta).shape
 
     """
+    if not isinstance(mu, Tensor) or not torch.is_floating_point(mu):
+        raise TypeError("mu must be a floating point tensor.")
+
     dtype = mu.dtype
     if n is None:
-        n = {torch.half: 4, torch.float: 5, torch.double: 6}[dtype]
+        n = {torch.bfloat16: 3, torch.half: 4, torch.float: 5, torch.double: 6}[dtype]
 
-    mu = mu.float() if n <= 5 else mu.double()
+    if n > 5:
+        mu = mu.double()
+    elif dtype in {torch.bfloat16, torch.half}:
+        mu = mu.float()  # torch.special.erfcx does not support bfloat16 or half
 
     umin = (V_r - mu) / sigma
     umax = (theta - mu) / sigma
 
     if (-umin).min() > -10:
         # slightly faster path when there is no extreme value
         out = 1 / (tau_rp + tau * sqrtpi * ierfcx(-umax, -umin, n=n))
```

### Comparing `ricciardi-0.1.2/src/ricciardi.egg-info/PKG-INFO` & `ricciardi-0.1.3/src/ricciardi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricciardi
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyTorch implementation of the Ricciardi transfer function.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,27 +25,34 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repository, https://github.com/hchau630/ricciardi
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: torch
 
+![tests workflow status](https://github.com/hchau630/ricciardi/actions/workflows/tests.yml/badge.svg)
+
 # About
 An efficient, GPU-friendly, and differentiable PyTorch implementation of the Ricciardi transfer function based on equations and default parameters from [Sanzeni et al. (2020)](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008165).
 
 # Usage
 For using the ricciardi function in your own code, you can either just copy the source file at `src/ricciardi/ricciardi.py` to your own code, or install the package in your python environment with `pip install ricciardi` and import the function with `from ricciardi import ricciardi`. To run tests, clone the repository, create a new environment, install the neccessary packages with `pip install -r requirements`, and run the command `pytest`.
 
 # Benchmark
-Compare performance with an interpolation-based approach. Forward pass is slightly slower, but backward pass is >2x faster on GPU.
+Compare performance with a naive, linear interpolation-based approach. Forward pass is slightly slower, but backward pass is >2x faster on GPU.
 
 Results on CPU (AMD EPYC 7662, 8 cores) (`python benchmark/benchmark.py -N 100000 -r 100`):
 ```
 forward pass, requires_grad=False
 ricciardi: median=1.86 ms, min=1.84 ms (100 repeats)
 ricciardi_interp: median=1.75 ms, min=1.72 ms (100 repeats)
```

### Comparing `ricciardi-0.1.2/test/test_ricciardi.py` & `ricciardi-0.1.3/test/test_ricciardi.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 @pytest.mark.parametrize(
     "x",
     [
         torch.linspace(-0.01, 0.1, 1001),
         torch.linspace(-10.0, 50.0, 1001),
     ],
 )
-@pytest.mark.parametrize("dtype", [torch.half, torch.float, torch.double])
+@pytest.mark.parametrize(
+    "dtype", [torch.bfloat16, torch.half, torch.float, torch.double]
+)
 def test_ricciardi(x, params, dtype):
     x = x.to(dtype)
     out = ricciardi(x, **params)
     expected = ricciardi_exact(x.double().numpy(), **params)
     expected = torch.from_numpy(expected).to(dtype).nan_to_num()
     torch.testing.assert_close(out, expected)
```

