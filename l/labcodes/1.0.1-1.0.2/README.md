# Comparing `tmp/labcodes-1.0.1.tar.gz` & `tmp/labcodes-1.0.2.tar.gz`

## Comparing `labcodes-1.0.1.tar` & `labcodes-1.0.2.tar`

### file list

```diff
@@ -1,52 +1,42 @@
--rw-r--r--   0        0        0   131011 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/Q_of_LC_CCoupled.ipynb
--rw-r--r--   0        0        0   122313 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/Q_of_LC_MCoupled.ipynb
--rw-r--r--   0        0        0   189862 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/all you need is pandas.ipynb
--rw-r--r--   0        0        0   195390 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/fitter_basic.ipynb
--rw-r--r--   0        0        0   143137 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/plot2d.ipynb
--rw-r--r--   0        0        0   193473 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/state_discrimination.ipynb
--rw-r--r--   0        0        0   290921 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/tomo.ipynb
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/__about__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/__init__.py
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/crosstalk.py
--rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/enr_cross.py
--rw-r--r--   0        0        0    13557 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fit_resonator.py
--rw-r--r--   0        0        0    24134 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fitter.py
--rw-r--r--   0        0        0    16865 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/misc.py
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/models.py
--rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/state_disc.py
--rw-r--r--   0        0        0    33230 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/tomo.py
--rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/app/mat_editor.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/__init__.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/base.py
--rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/qubits.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/resonator_qc.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/__init__.py
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/base.py
--rw-r--r--   0        0        0    23160 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/labber.py
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/labrad.py
--rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/ltspice.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/misc.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/benchmark.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/iq_scatter.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/labrad_timefunc2freq.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/pulse_calc.py
--rw-r--r--   0        0        0    35424 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/routine.py
--rw-r--r--   0        0        0    57486 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/state_list.py
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele.py
--rw-r--r--   0        0        0    10784 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele_gate.py
--rw-r--r--   0        0        0    15959 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele_state.py
--rw-r--r--   0        0        0    30003 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele_swep.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/__init__.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/matrix.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/misc.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/plot2d.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/rt_qst_qpt.py
--rw-r--r--   0        0        0    83813 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/data/00003 - power shift.csv
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/data/00003 - power shift.ini
--rw-r--r--   0        0        0    71586 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/data/fit_resonator.feather
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 labcodes-1.0.1/.gitignore
--rw-r--r--   0        0        0    35813 2020-02-02 00:00:00.000000 labcodes-1.0.1/LICENSE
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 labcodes-1.0.1/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 labcodes-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 labcodes-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/__about__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/__init__.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/crosstalk.py
+-rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/enr_cross.py
+-rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fit_resonator.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fitter.py
+-rw-r--r--   0        0        0    16865 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/misc.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/models.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/peak_find.py
+-rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/state_disc.py
+-rw-r--r--   0        0        0    33230 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/tomo.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/app/mat_editor.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/calc/__init__.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/calc/base.py
+-rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/calc/qubits.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/calc/resonator_qc.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fileio/__init__.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fileio/base.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fileio/labber.py
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fileio/labrad.py
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fileio/ltspice.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/fileio/misc.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/benchmark.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/iq_scatter.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/labrad_timefunc2freq.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/pulse_calc.py
+-rw-r--r--   0        0        0    35424 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/routine.py
+-rw-r--r--   0        0        0    57486 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/state_list.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/tele.py
+-rw-r--r--   0        0        0    10784 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/tele_gate.py
+-rw-r--r--   0        0        0    15959 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/tele_state.py
+-rw-r--r--   0        0        0    30003 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/frog/tele_swep.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/plotter/__init__.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/plotter/matrix.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/plotter/misc.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 labcodes-1.0.2/labcodes/plotter/plot2d.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 labcodes-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35813 2020-02-02 00:00:00.000000 labcodes-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 labcodes-1.0.2/README.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 labcodes-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 labcodes-1.0.2/PKG-INFO
```

### Comparing `labcodes-1.0.1/labcodes/crosstalk.py` & `labcodes-1.0.2/labcodes/crosstalk.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/enr_cross.py` & `labcodes-1.0.2/labcodes/enr_cross.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from labcodes import misc, plotter
 from labcodes.calc import Calculator, dept
 from scipy.signal import find_peaks
 
-logger = logging.getLogger(__file__)
+logger = logging.getLogger(__name__)
 
 
 class EnrCross(Calculator):
     """Model for the avoid level crossing on spectrums."""
 
     x = np.linspace(3.5, 4.5, 21)
     g = 0.1
```

### Comparing `labcodes-1.0.1/labcodes/fit_resonator.py` & `labcodes-1.0.2/labcodes/fit_resonator.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import lmfit
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy.constants as const
 
 from labcodes import misc, plotter
+from labcodes.peak_find import PeakFinder
 
-logger = logging.getLogger(__file__)
+logger = logging.getLogger(__name__)
 
 
 def s21m1(x, Qi=1e6, Qc=1e3, f0=4, phi=0, alpha=-50, phiv=10, phi0=0, amp=1):
     """Normalized s21^-1 for linear resonator.
 
     Original paper see https://doi.org/10.1063/1.3693409
     Improved by Xiayu Linpeng.
@@ -43,75 +44,112 @@
 
     Adapted from:
     1. https://lmfit.github.io/lmfit-py/examples/example_complex_resonator_model.html
     2. programs by Xiayu Linpeng.
     """
 
     def __init__(
-        self, freq: np.ndarray, s21_dB: np.ndarray, s21_rad: np.ndarray, **fit_kws
+        self,
+        freq: np.ndarray = None,
+        s21_dB: np.ndarray = None,
+        s21_rad: np.ndarray = None,
+        df: pd.DataFrame = None,
+        hold: bool = False,
+        **fit_kws,
     ):
-        """fit(Qi=1e6) to overwrite initial guess."""
-        # Normalize data with y0=0.
-        s21_rad = np.unwrap(s21_rad)
-        s21_dB = remove_background(s21_dB, freq, fit_mask=100, offset=0)
-        s21_rad = remove_background(s21_rad, freq, fit_mask=100, offset=0)
-        s21_cplx = 10 ** (s21_dB / 20) * np.exp(1j * s21_rad)
-        s21m1_cplx = 1 / s21_cplx
-        self.df = pd.DataFrame(
-            dict(
-                freq=freq,
-                s21_dB=s21_dB,
-                s21_rad=s21_rad,
-                s21_cplx=s21_cplx,
-                s21m1_cplx=s21m1_cplx,
-            )
-        )
+        """Prepare data, guess initial parameters, then fit.
+        
+        Usage:
+
+        - To skip data preparation, provide `df`.
+
+        - To manually set initial guess, pass values like `fit(Qi=1e6)`.
+
+        - One can always modify `df`, `init_params` then call `fit()` again to custom the fit.
+        """
+        if df is None:
+            self.df = self.prepare_data(freq, s21_dB, s21_rad)
+        else:
+            self.df = df.copy()[['freq', 's21_dB', 's21_rad']]
+
         self.init_params = None
-        self.guess_and_update_params()
+        self.init_params = self.guess_params()
+
         self.result: lmfit.minimizer.MinimizerResult = None
-        try:
-            self.fit(**fit_kws)
-        except:
-            logger.exception("Error in fitting.")
+        if not hold:
+            try:
+                self.fit(**fit_kws)
+            except:
+                logger.exception("Error in fitting.")
+
+    @staticmethod
+    def prepare_data(freq: np.ndarray, s21_dB: np.ndarray, s21_rad: np.ndarray):
+        freq = np.asarray(freq)
+        s21_dB = np.asarray(s21_dB)
+        s21_rad = np.asarray(s21_rad)
+
+        n_pts_bg = freq.size // 10
+        s21_rad = np.unwrap(s21_rad)
+        s21_dB = remove_background(s21_dB, freq, fit_mask=n_pts_bg, offset=0)
+        s21_rad = remove_background(s21_rad, freq, fit_mask=slice(0, n_pts_bg), 
+                                    offset=0)
+
+        return pd.DataFrame(dict(freq=freq, s21_dB=s21_dB, s21_rad=s21_rad))
+    
+    @property
+    def s21_cplx(self) -> np.ndarray:
+        return self.df.eval('10 ** (s21_dB / 20) * exp(1j * s21_rad)').values
 
     def fit(self, **fit_kws) -> lmfit.minimizer.MinimizerResult:
-        """fit(Qi=1e6) to overwrite initial guess."""
+        """fit(Qi=1e6) to overwrite initial guess.
+        
+        Defaultly uses `weights=np.abs(s21_cplx)`. Pass `weights=None` to disable any weights.
+        """
         freq = self.df.freq.values
-        s21m1_cplx = self.df.s21m1_cplx.values
+        s21_cplx = self.s21_cplx
+        s21m1_cplx = 1 / s21_cplx
+
+        if 'weights' not in fit_kws:
+            # Lower weight around dip, for improved robustness with noisy data.
+            # pass weights=None to disable any weights.
+            fit_kws['weights'] = np.abs(s21_cplx)
 
         self.result = model.fit(
             s21m1_cplx,
             x=freq,
             params=self.init_params,
-            # weights=np.abs(s21m1_cplx),  # not necessary.
             method="Powell",
             **fit_kws,
         )
         return self.result
 
-    def guess_and_update_params(self):
+    def guess_params(self):
         freq = self.df.freq.values
         s21_dB = self.df.s21_dB.values
-        s21_cplx = self.df.s21_cplx.values
-        s21m1_cplx = self.df.s21m1_cplx.values
+        s21_cplx = self.s21_cplx
+        s21m1_cplx = 1 / s21_cplx
 
         idip = np.argmin(s21_dB)
         fr = freq[idip]
 
-        Qc = guess_Qc(s21_cplx, freq, fr, idip, s21_dB)
-        Qi = guess_Qi(s21m1_cplx, freq, fr, idip)
+        pf = PeakFinder(freq, -np.abs(s21_cplx))
+        Qc = abs(pf['center'] / pf['hwhm']) / 2
+
+        pf = PeakFinder(freq, np.abs(s21m1_cplx))
+        Qi = abs(pf['center'] / pf['hwhm'])
+        if np.sum(np.real(s21m1_cplx)) < 1:
+            Qi = -Qi
 
         freq_span = freq[-1] - freq[0]
         alpha = fr * (abs(s21_cplx[-1]) - abs(s21_cplx[0])) / freq_span
         phiv = np.angle(s21m1_cplx[-1] / s21m1_cplx[0]) / freq_span
 
         params = lmfit.Parameters()
         params.set(Qi=Qi, Qc=Qc, f0=fr, phi=0, alpha=alpha, phiv=phiv, phi0=0, amp=1)
         params.set(phiv=dict(min=-np.pi / freq_span, max=np.pi / freq_span))
-        self.init_params = params
         return params
 
     def __getitem__(self, key: str):
         if self.result is not None:
             if key == "chi":
                 return np.sqrt(self.result.chisqr)
             elif key.endswith("_err"):
@@ -146,32 +184,34 @@
             setup_ax_cplx(ax)
         if freq is None:
             freq = self.df.freq.values
 
         f0 = self["f0"]
         Qi = self["Qi"]
         Qc = self["Qc"]
-        dfi = f0 / Qi / 2
-        dfc = f0 / Qc / 2
+        dfi = abs(f0 / Qi / 2)
+        dfc = abs(f0 / Qc / 2)
 
         def plot(ax: plt.Axes, x: np.ndarray, y: np.ndarray, sty="-", **kw):
             dx = np.abs(x - f0)
             mask1 = dx <= dfi
-            mask3 = dx >= dfi * 10
+            mask3 = dx >= dfc
             mask2 = np.logical_not(mask1 | mask3)
             ax.plot(y.real[mask1], y.imag[mask1], sty, color="C0", **kw)
             ax.plot(y.real[mask2], y.imag[mask2], sty, color="C1", **kw)
             ax.plot(y.real[mask3], y.imag[mask3], sty, color="C2", **kw)
 
-        plot(ax, self.df.freq.values, self.df.s21m1_cplx.values, ".", alpha=0.5)
+        plot(ax, self.df.freq.values, 1 / self.s21_cplx, ".", alpha=0.5)
 
         if (self.result is not None) and plot_fit:
             plot(ax, freq, self.result.eval(x=freq), "-")
             ax.annotate(
-                f"$f_0$={misc.estr(f0)}\n$Q_i$={misc.estr(Qi)}\n$Q_c$={misc.estr(Qc)}",
+                (f"$f_0={f0:.4g}$\n"
+                 f"$Q_i={Qi:+.4g}$\n"
+                 f"$Q_c={Qc:+.4g}$"),
                 (0.5, 0.5),
                 xycoords="axes fraction",
                 ha="center",
                 va="center",
             )
 
         if plot_init:
@@ -186,55 +226,55 @@
         freq: np.ndarray = None,
         plot_fit: bool = True,
         plot_init: bool = False,
     ):
         if axs is None:
             _, (ax, ax2) = plt.subplots(figsize=(6, 2), ncols=2)
             setup_ax_abs(ax)
-            setup_ax_rad(ax2)
+            setup_ax_deg(ax2)
         else:
             ax, ax2 = axs
 
         if freq is None:
             freq = self.df.freq.values
 
         f0 = self["f0"]
         Qi = self["Qi"]
         Qc = self["Qc"]
-        dfi = f0 / Qi / 2
-        dfc = f0 / Qc / 2
+        dfi = abs(f0 / Qi / 2)
+        dfc = abs(f0 / Qc / 2)
 
         def plot(ax: plt.Axes, x: np.ndarray, y: np.ndarray, sty="-"):
             dx = np.abs(x - f0)
             mask1 = dx <= dfi
-            mask3 = dx >= dfi * 10
+            mask3 = dx >= dfc
             mask2 = np.logical_not(mask1 | mask3)
             mask2a = mask2 & (x < f0)
             mask2b = mask2 & (x >= f0)
             mask3a = mask3 & (x < f0)
             mask3b = mask3 & (x >= f0)
             ax.plot(x[mask1], y[mask1], sty, color="C0")
             ax.plot(x[mask2a], y[mask2a], sty, color="C1")
             ax.plot(x[mask2b], y[mask2b], sty, color="C1")
             ax.plot(x[mask3a], y[mask3a], sty, color="C2")
             ax.plot(x[mask3b], y[mask3b], sty, color="C2")
 
         plot(ax, self.df.freq.values, self.df.s21_dB.values, ".")
-        plot(ax2, self.df.freq.values, self.df.s21_rad.values, ".")
+        plot(ax2, self.df.freq.values, np.rad2deg(self.df.s21_rad.values), ".")
 
         if (self.result is not None) and plot_fit:
             s21_cplx = 1 / self.result.eval(x=freq)
             ax.plot(freq, 20 * np.log10(np.abs(s21_cplx)), "k-")
-            ax2.plot(freq, np.angle(s21_cplx), "k-")
+            ax2.plot(freq, np.rad2deg(np.unwrap(np.angle(s21_cplx))), "k-")
 
         if plot_init:
             init_param = {k: p.init_value for k, p in self.result.params.items()}
             s21_cplx = 1 / model.eval(x=freq, **init_param)
             ax.plot(freq, 20 * np.log10(np.abs(s21_cplx)), "--", color="gray")
-            ax2.plot(freq, np.angle(s21_cplx), "--", color="gray")
+            ax2.plot(freq, np.rad2deg(np.unwrap(np.angle(s21_cplx))), "--", color="gray")
 
         return ax, ax2
 
     def plot(
         self,
         axs: tuple[plt.Axes, plt.Axes, plt.Axes] = None,
         freq: np.ndarray = None,
@@ -242,15 +282,15 @@
         plot_init: bool = False,
     ):
         if axs is None:
             _, (ax, ax2, ax3) = plt.subplots(
                 figsize=(8, 3), ncols=3, layout="constrained"
             )
             setup_ax_abs(ax)
-            setup_ax_rad(ax2)
+            setup_ax_deg(ax2)
             setup_ax_cplx(ax3)
         else:
             ax, ax2, ax3 = axs
 
         self.plot_cplx(ax=ax3, freq=freq, plot_fit=plot_fit, plot_init=plot_init)
         self.plot_s21(axs=(ax, ax2), freq=freq, plot_fit=plot_fit, plot_init=plot_init)
         return ax, ax2, ax3
@@ -260,19 +300,24 @@
     ax.set_xlabel("freq")
     ax.set_title("s21_dB")
 
 
 def setup_ax_rad(ax: plt.Axes):
     ax.set_xlabel("freq")
     ax.set_title("s21_rad")
-    ax.set_ylim(-3.2, 3.2)
+    # ax.set_ylim(-3.2, 3.2)
     ax.yaxis.set_major_locator(plt.MultipleLocator(np.pi / 2))
     ax.yaxis.set_major_formatter(plotter.misc.multiple_formatter(2, np.pi))
 
 
+def setup_ax_deg(ax: plt.Axes):
+    ax.set_xlabel("freq")
+    ax.set_title("s21_deg")
+
+
 def setup_ax_cplx(ax: plt.Axes):
     ax.set_xlabel("Re[$S_{21}^{-1}$]")
     ax.set_ylabel("Im[$S_{21}^{-1}$]")
     ax.set_aspect("equal")
     ax.axhline(y=0, color="gray", alpha=0.5, zorder=1)
     ax.axvline(x=1, color="gray", alpha=0.5, zorder=1)
 
@@ -321,112 +366,19 @@
         ax.plot(x, y_fit, label="bg")
         ax.plot(x, new_y, label="new")
         ax.legend()
         plt.show()
     return new_y
 
 
-def lorentz(x, center, width, amp, offset):
-    return amp * width / ((x - center) ** 2 + width**2) + offset
-
-
-def lorentz_m1(x, center, width, amp, offset):
-    return 1 - amp * width / ((x - center) ** 2 + width**2) + offset
-
-
-model_lorentz = lmfit.Model(lorentz)
-model_lorentz_m1 = lmfit.Model(lorentz_m1)
-
-
-def guess_Qi(
-    s21m1_cplx: np.ndarray,
-    freq: np.ndarray,
-    fr: float,
-    idip: int = None,
-):
-    s21m1_abs = np.abs(s21m1_cplx)
-    if idip is None:
-        idip = np.argmax(s21m1_abs)
-    if idip == 0:
-        logger.warn("fr <= freq.")
-        idip = 1
-    if idip == np.size(freq):
-        logger.warn("fr >= freq.")
-        idip = -2
-
-    half_maximum = (s21m1_abs[idip] + 1) / 2
-    fwhm = 0.1 * np.abs(  # Emprical value.
-        freq[np.argmin(np.abs(s21m1_abs[:idip] - half_maximum))]
-        - freq[np.argmin(np.abs(s21m1_abs[idip:] - half_maximum))]
-    )
-    Qi = np.abs(fr / fwhm)
-
-    try:
-        res = model_lorentz.fit(
-            s21m1_abs,
-            x=freq,
-            center=fr,
-            width=fwhm / 5,
-            amp=0.1 * (s21m1_abs[idip] - 1),
-            offset=1,
-        )
-        Qi = np.abs(res.params["center"].value / res.params["width"].value)
-    except:
-        logger.warn("Fail to fit Lorentz in guessing Qi.")
-
-    if np.mean(np.real(s21m1_cplx)) < 1:
-        Qi = -Qi
-
-    return Qi
-
-
-def guess_Qc(
-    s21_cplx: np.ndarray,
-    freq: np.ndarray,
-    fr: float,
-    idip: int = None,
-    s21_dB: np.ndarray = None,
-):
-    s21_abs = np.abs(s21_cplx)
-    if idip is None:
-        idip = np.argmin(s21_abs)
-    if idip == 0:
-        logger.warn("fr <= freq.")
-        idip = 1
-    if idip == np.size(freq):
-        logger.warn("fr >= freq.")
-        idip = -2
-
-    if s21_dB is None:
-        s21_dB = 20 * np.log10(s21_abs)
-
-    half_maximum = s21_dB[idip] + 3
-    fwhm = 0.2 * np.abs(  # Emprical value.
-        freq[np.argmin(np.abs(s21_dB[:idip] - half_maximum))]
-        - freq[np.argmin(np.abs(s21_dB[idip:] - half_maximum))]
-    )
-    Qc = np.abs(fr / fwhm)
-
-    try:
-        res = model_lorentz_m1.fit(
-            s21_cplx,
-            x=freq,
-            center=fr,
-            width=fwhm / 2,
-            amp=1 - s21_abs[idip],
-            offset=0,
-        )
-        Qc = np.abs(res.params["center"].value / res.params["width"].value / 2)
-    except:
-        logger.warn("Fail to fit Lorentz in guessing Qc.")
-
-    return Qc
-
 
 if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
+
     freq = misc.segments(
         misc.center_span(4, 0.01e-3, n=101),
         misc.center_span(4, 10e-3, n=101),
     )
     freq = np.sort(freq)
     s21m1_cplx = s21m1(freq)
     s21_cplx = 1 / s21m1_cplx
```

### Comparing `labcodes-1.0.1/labcodes/fitter.py` & `labcodes-1.0.2/labcodes/fitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -641,10 +641,45 @@
     xbatch = x_series.to_list()
     ybatch = y_series.to_list()
     stepper_value = x_series.index
 
     return xbatch, ybatch, stepper_value
 
 
+def resample(y: np.ndarray, n_pts: int) -> np.ndarray:
+    """Return yp by resampling y for n_pts points.
+
+    >>> resample([0, 3, 33], 7)
+    array([ 0.,  1.,  2.,  3., 13., 23., 33.])
+    """
+    y = np.ravel(y)
+    x = np.linspace(0, 1, num=len(y))
+    xp = np.linspace(0, 1, num=n_pts)
+    return np.interp(xp, x, y)
+
+
+def getitem_from_fit_result(res: lmfit.model.ModelResult, k: str) -> float:
+    """Get parameter value or stderr from a fit result.
+
+    For quick implementation of __getitem__ of fitters.
+    """
+    if res is None:
+        raise ValueError("No valid result yet.")
+
+    if k == "chi":
+        return np.sqrt(res.chisqr)
+    elif k in res.model.param_names:
+        return res.params[k].value
+    elif k.removesuffix("_err") in res.model.param_names:
+        k = k.removesuffix("_err")
+        v = res.params[k].stderr
+        if v is None:
+            return np.nan
+        else:
+            return v
+    else:
+        raise KeyError("Invalid key: %s", k)
+
+
 if __name__ == '__main__':
     import doctest
     doctest.testmod()
```

### Comparing `labcodes-1.0.1/labcodes/misc.py` & `labcodes-1.0.2/labcodes/misc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/models.py` & `labcodes-1.0.2/labcodes/models.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/state_disc.py` & `labcodes-1.0.2/labcodes/state_disc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/tomo.py` & `labcodes-1.0.2/labcodes/tomo.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/app/mat_editor.py` & `labcodes-1.0.2/labcodes/app/mat_editor.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/calc/__init__.py` & `labcodes-1.0.2/labcodes/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/calc/base.py` & `labcodes-1.0.2/labcodes/calc/base.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/calc/qubits.py` & `labcodes-1.0.2/labcodes/calc/qubits.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/calc/resonator_qc.py` & `labcodes-1.0.2/labcodes/calc/resonator_qc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/fileio/base.py` & `labcodes-1.0.2/labcodes/fileio/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import json
 import textwrap
 from copy import copy
 from pathlib import Path
-from typing import Union, Literal
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from attrs import define
 
-from labcodes.fileio.misc import data_from_json, data_to_json
 from labcodes import plotter
+from labcodes.fileio.misc import data_from_json, data_to_json
 
 PATH_LEGAL = {
     "->": "→",
     "<-": "←",
     ":": ",",
     "|": "l",
     # '?': '？',
@@ -40,18 +38,26 @@
     def plot(self, **kwargs):
         """Quick data plot."""
         if len(self.indeps) == 1:
             return self.plot1d(**kwargs)
         else:
             return self.plot2d(**kwargs)
 
-    def plot1d(self, x_name=0, y_name=0, ax: plt.Axes = None, **kwargs):
+    def plot1d(
+        self,
+        x_name: str | int = 0,
+        y_name: str | int = 0,
+        ax: plt.Axes = None,
+        **kwargs,
+    ):
         """Quick line plot."""
+        set_ax_label: bool = False
         if ax is None:
             _, ax = plt.subplots()
+            set_ax_label = True
 
         if isinstance(x_name, int):
             x_name = self.indeps[x_name]
         # convert y_name to list(str)
         if not isinstance(y_name, list):
             y_name = [y_name]
         if isinstance(y_name[0], int):
@@ -65,38 +71,43 @@
 
         kw = dict(marker=".")
         kw.update(kwargs)
 
         for yn, lb in zip(y_name, labels):
             ax.plot(x_name, yn, data=self.df, label=lb, **kw)
 
-        if np.size(y_name) > 1:
-            ax.legend()
-        ax.grid(True)
-        ax.set_title(self.name.ptitle())
-        ax.set_xlabel(x_name)
-        ax.set_ylabel(y_name[0])
-        return ax
-
-    def plot2d(self, x_name=0, y_name=1, z_name=0, ax: plt.Axes = None, **kwargs):
-        """Quick 2d plot with plotter.plot2d_[kind]."""
-        if ax is None:
-            _, ax = plt.subplots()
-            ax.set_title(self.name.as_plot_title())
+        if set_ax_label:
+            if np.size(y_name) > 1:
+                ax.legend()
+            ax.grid(True)
+            ax.set_title(self.name.ptitle())
             ax.set_xlabel(x_name)
-            ax.set_ylabel(y_name)
+            ax.set_ylabel(y_name[0])
+        return ax
 
+    def plot2d(
+        self,
+        x_name: str | int = 0,
+        y_name: str | int = 1,
+        z_name: str | int = 0,
+        ax: plt.Axes = None,
+        **kwargs,
+    ):
+        """Quick 2d plot with plotter.plot2d_auto."""
         if isinstance(x_name, int):
             x_name = self.indeps[x_name]
         if isinstance(y_name, int):
             y_name = self.indeps[y_name]
         if isinstance(z_name, int):
             z_name = self.deps[z_name]
 
-        plotter.plot2d_auto(self.df, x_name=x_name, y_name=y_name, z_name=z_name, ax=ax, **kwargs)
+        ax = plotter.plot2d_auto(
+            self.df, x_name=x_name, y_name=y_name, z_name=z_name, ax=ax, **kwargs
+        )
+        ax.set_title(self.name.as_plot_title())
 
         return ax
 
     @classmethod
     def load(cls, dir: Path, id: int) -> "LogFile":
         """Load a logfile from a .feather and a .json files."""
         dir = Path(dir)
@@ -107,15 +118,15 @@
         indeps = conf["indeps"]
         deps = conf["deps"]
         return cls(df=df, conf=conf, name=name, indeps=indeps, deps=deps)
 
     def save(self, dir: Path) -> Path:
         """Save a logfile into a .feather file and a .json files."""
         dir = Path(dir).resolve()
-        p = dir / (self.name.fname() + '.no_suffix')
+        p = dir / (self.name.fname() + ".no_suffix")
         self.df.to_feather(p.with_suffix(".feather"))
 
         conf = self.conf.copy()
         if "deps" not in conf:
             conf["deps"] = self.deps
         if "indeps" not in conf:
             conf["indeps"] = self.indeps
@@ -172,16 +183,16 @@
 class LogName:
     """A LogName.fname looks like: #[id], [title].suffix.
 
     suffix could be csv, ini, json, feather, png, jpg, svg...
     id could be '12' or '1,2,3' or '1-4'.
     """
 
-    dir: Union[str, Path]
-    id: Union[str, int]
+    dir: str | Path
+    id: str | int
     title: str
 
     def __str__(self):
         return f"#{self.id}, {self.title}"
 
     def as_plot_title(self, width: int = 60) -> str:
         s = f"#{self.id}, {self.title}"
@@ -191,36 +202,36 @@
         # f = textwrap.fill(f, width=width)
 
         s = f"{f}\\\n{s}"
         return s
 
     ptitle = as_plot_title
 
-    def as_file_name(self, suffix: str = '') -> str:
+    def as_file_name(self, suffix: str = "") -> str:
         s = f"#{self.id}, {self.title}"
         for k, v in PATH_LEGAL.items():
             s = s.replace(k, v)
         if suffix:
             s += suffix
         return s
 
     fname = as_file_name
 
     @classmethod
-    def from_path(cls, p: Union[str, Path]) -> "LogName":
+    def from_path(cls, p: str | Path) -> "LogName":
         p = Path(p)
         dir = p.parent
         id, title = p.stem[1:].split(", ", 1)
         return cls(dir=dir, id=id, title=title)
 
-    def copy(self, id: Union[str, int] = None, title: str = None) -> "LogName":
+    def copy(self, id: str | int = None, title: str = None) -> "LogName":
         name = copy(self)
         if id is not None:
             name.id = id
         if title is not None:
             name.title = title
         return name
 
-    def save_aside_data(self, fig: Union[plt.Axes, plt.Figure]) -> None:
+    def save_aside_data(self, fig: plt.Axes | plt.Figure) -> None:
         if isinstance(fig, plt.Axes):
             fig = fig.get_figure()
         fig.savefig(self.dir / (self.as_file_name() + ".png"))
```

### Comparing `labcodes-1.0.1/labcodes/fileio/labrad.py` & `labcodes-1.0.2/labcodes/fileio/labrad.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/fileio/ltspice.py` & `labcodes-1.0.2/labcodes/fileio/ltspice.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/benchmark.py` & `labcodes-1.0.2/labcodes/frog/benchmark.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/iq_scatter.py` & `labcodes-1.0.2/labcodes/frog/iq_scatter.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/labrad_timefunc2freq.py` & `labcodes-1.0.2/labcodes/frog/labrad_timefunc2freq.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/pulse_calc.py` & `labcodes-1.0.2/labcodes/frog/pulse_calc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/routine.py` & `labcodes-1.0.2/labcodes/frog/routine.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/state_list.py` & `labcodes-1.0.2/labcodes/frog/state_list.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/tele.py` & `labcodes-1.0.2/labcodes/frog/tele.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/tele_gate.py` & `labcodes-1.0.2/labcodes/frog/tele_gate.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/tele_state.py` & `labcodes-1.0.2/labcodes/frog/tele_state.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/frog/tele_swep.py` & `labcodes-1.0.2/labcodes/frog/tele_swep.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/plotter/__init__.py` & `labcodes-1.0.2/labcodes/plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/plotter/matrix.py` & `labcodes-1.0.2/labcodes/plotter/matrix.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/plotter/misc.py` & `labcodes-1.0.2/labcodes/plotter/misc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/labcodes/plotter/plot2d.py` & `labcodes-1.0.2/labcodes/plotter/plot2d.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/.gitignore` & `labcodes-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/LICENSE` & `labcodes-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/README.md` & `labcodes-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.1/pyproject.toml` & `labcodes-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     "matplotlib",
     "pandas",
     "lmfit>=0.9.5",
     # 'h5py>=2.6',
     "tqdm",
     "attrs",
     # 'dpath',
-    # 'PyQt5',  # requirements of Labber API here and below.
     "json-numpy",
     "cvxpy",  # for tomography.
     "scikit-learn",  # for state_disc.
     "cmocean",  # for matrix plot.
 ]
 requires-python = ">=3.9"
 authors = [{ name = "Qiujv", email = "qiujv@outlook.com" }]
@@ -35,7 +34,14 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["labcodes"]
 
 [tool.hatch.version]
 path = "labcodes/__about__.py"
+
+[tool.hatch.build.targets.sdist]
+exclude = [
+  "/data",
+  "/examples",
+  "/tests",
+]
```

### Comparing `labcodes-1.0.1/PKG-INFO` & `labcodes-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labcodes
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple routines for superconducting quantum circuits.
 Project-URL: Homepage, https://github.com/Qiujv/LabCodes
 Author-email: Qiujv <qiujv@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

