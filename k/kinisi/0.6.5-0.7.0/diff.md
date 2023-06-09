# Comparing `tmp/kinisi-0.6.5.tar.gz` & `tmp/kinisi-0.7.0.tar.gz`

## Comparing `kinisi-0.6.5.tar` & `kinisi-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/analyze.py
--rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/analyzer.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/arrhenius.py
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/conductivity_analyzer.py
--rw-r--r--   0        0        0    34779 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/diffusion.py
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/diffusion_analyzer.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/jump_diffusion_analyzer.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/matrix.py
--rw-r--r--   0        0        0    23518 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/__init__.py
--rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_analyze.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_arrhenius.py
--rw-r--r--   0        0        0    38583 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_diffusion.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_matrix.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_parser.py
--rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.data
--rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.dcd
--rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/inputs/example_XDATCAR.gz
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.6.5/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.6.5/LICENSE
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.6.5/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 kinisi-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 kinisi-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/analyze.py
+-rw-r--r--   0        0        0    19195 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/analyzer.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/arrhenius.py
+-rw-r--r--   0        0        0    15042 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/conductivity_analyzer.py
+-rw-r--r--   0        0        0    35056 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/diffusion.py
+-rw-r--r--   0        0        0    13062 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/diffusion_analyzer.py
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/jump_diffusion_analyzer.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/matrix.py
+-rw-r--r--   0        0        0    29472 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/__init__.py
+-rw-r--r--   0        0        0    17448 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/test_analyze.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/test_arrhenius.py
+-rw-r--r--   0        0        0    38650 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/test_diffusion.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/test_matrix.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/test_parser.py
+-rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/inputs/example_LAMMPS.data
+-rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/inputs/example_LAMMPS.dcd
+-rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/inputs/example_XDATCAR.gz
+-rw-r--r--   0        0        0  4297126 2020-02-02 00:00:00.000000 kinisi-0.7.0/kinisi/tests/inputs/example_ase.traj
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.7.0/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 kinisi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 kinisi-0.7.0/PKG-INFO
```

### Comparing `kinisi-0.6.5/kinisi/analyze.py` & `kinisi-0.7.0/kinisi/analyze.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/kinisi/analyzer.py` & `kinisi-0.7.0/kinisi/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Copyright (c) Andrew R. McCluskey and Benjamin J. Morgan
 # Distributed under the terms of the MIT License
 # author: Andrew R. McCluskey (arm61)
 
 from typing import Union, List
 import numpy as np
-from kinisi.parser import MDAnalysisParser, PymatgenParser
+from kinisi.parser import MDAnalysisParser, PymatgenParser, ASEParser
 
 
 class Analyzer:
     """
     This class is the superclass for the :py:class:`kinisi.analyze.DiffusionAnalyzer`,
     :py:class:`kinisi.analyze.JumpDiffusionAnalyzer` and :py:class:`kinisi.analyze.ConductivityAnalyzer` classes.
     Therefore all of the properties here are available to these other classes.
@@ -32,16 +32,15 @@
 
     def save(self, filename: str):
         """
         Save the Analyzer object as a HDF5 file.
 
         :param filename: Name for the file, no file extension is required and if one if given it is replaced with .hdf.
         """
-        if filename[-4:] != '.hdf':
-            raise ValueError("The expected file extension is .hdf")
+        filename = filename.rsplit('.', 1)[0] + '.hdf'
         my_dict = self.to_dict()
         try:
             import h5py
             from os.path import exists
         except ModuleNotFoundError:  # pragma: no cover
             raise ModuleNotFoundError("To save and load objects, the h5py module is required")  # pragma: no cover
         if exists(filename):
@@ -54,16 +53,15 @@
         """
         Load the :py:class:`Analyzer` object from an HDF5 file.
 
         :param filename: Name for the file, any file extension will be replaced with .hdf.
 
         :return: An :py:class:`Analyzer` object from the file.
         """
-        if filename[-4:] != '.hdf':
-            raise ValueError("The expected file extension is .hdf")
+        filename = filename.rsplit('.', 1)[0] + '.hdf'
         try:
             import h5py
         except ModuleNotFoundError:  # pragma: no cover
             raise ModuleNotFoundError("To save and load objects, the h5py module is required")  # pragma: no cover
         with h5py.File(filename, 'r') as h5file:
             my_dict = _group_to_dict(h5file, '/')
         return cls.from_dict(my_dict)
@@ -118,14 +116,52 @@
             return cls(u[0].delta_t, cls._stack_trajectories(u), n_o, u[0].volume, **kwargs)
         elif dtype == 'consecutive':
             structures = _flatten_list([x for x in trajectory])
             u = PymatgenParser(structures, **parser_params)
             return cls(u.delta_t, u.disp_3d, u._n_o, u.volume, **kwargs)
         else:
             raise ValueError('The dtype specified was not recognised, please consult the kinisi documentation.')
+        
+    @classmethod
+    def _from_ase(cls,
+                       trajectory: List[Union['ase.atoms.Atoms',
+                                              List['ase.atoms.Atoms']]],
+                       parser_params: dict,
+                       dtype: str = None,
+                       **kwargs):
+        """
+        Create a :py:class:`Analyzer` object from a list or nested list of
+        :py:class:`ase.atoms.Atoms` objects.
+
+        :param trajectory: The list or nested list of structures to be analysed.
+        :param parser_params: The parameters for the :py:class:`kinisi.parser.ASEParser` object.
+            See the appropriate documentation for more guidance on this dictionary.
+        :param dtype: If :py:attr:`trajectory` is a list of :py:class:`ase.atoms.Atoms`
+            objects, this should be :py:attr:`None`. However, if a list of lists is passed, then it is necessary
+            to identify if these constitute a series of :py:attr:`consecutive` trajectories or a series of
+            :py:attr:`identical` starting points with different random seeds, in which case the `dtype` should
+            be either :py:attr:`consecutive` or :py:attr:`identical`.
+
+        :return: Relevant :py:class:`Analyzer` object.
+        """
+        if dtype is None:
+            u = ASEParser(trajectory, **parser_params)
+            return cls(u.delta_t, u.disp_3d, u._n_o, u.volume, **kwargs)
+        elif dtype == 'identical':
+            u = [ASEParser(f, **parser_params) for f in trajectory]
+            n_o = np.zeros(u[0]._n_o.size)
+            for i in u:
+                n_o += i._n_o
+            return cls(u[0].delta_t, cls._stack_trajectories(u), n_o, u[0].volume, **kwargs)
+        elif dtype == 'consecutive':
+            structures = _flatten_list([x for x in trajectory])
+            u = ASEParser(structures, **parser_params)
+            return cls(u.delta_t, u.disp_3d, u._n_o, u.volume, **kwargs)
+        else:
+            raise ValueError('The dtype specified was not recognised, please consult the kinisi documentation.')
 
     @classmethod
     def _from_Xdatcar(cls,
                       trajectory: Union['pymatgen.io.vasp.outputs.Xdatcar', List['pymatgen.io.vasp.outputs.Xdatcar']],
                       parser_params: dict,
                       dtype: str = None,
                       **kwargs):
@@ -205,15 +241,15 @@
                        dtype: str = None,
                        **kwargs):
         """
         Create an :py:class:`Analyzer` object from an :py:class:`MDAnalysis.core.universe.Universe` object.
 
         :param trajectory: The universe to be analysed.
         :param parser_params: The parameters for the :py:class:`kinisi.parser.MDAnalysisParser` object.
-            See the appropriate documention for more guidance on this dictionary.
+            See the appropriate documentation for more guidance on this dictionary.
         :param dtype: If :py:attr:`trajectory` is a single file, this should be :py:attr:`None`. However, if a
             list of files is passed, then it is necessary to identify that these constitute a series of
             :py:attr:`identical` starting points with different random seeds, in which case the `dtype` should
             be :py:attr:`identical`. For a series of consecutive trajectories, please construct the relevant
             object using :py:mod:`MDAnalysis`.
 
         :return: Relevant :py:class:`Analyzer` object.
@@ -234,15 +270,15 @@
             return cls(u[0].delta_t, cls._stack_trajectories(u), n_o, u[0].volume, **kwargs)
         else:
             raise ValueError('The dtype specified was not recognised, please consult the kinisi documentation.')
 
     @staticmethod
     def _stack_trajectories(u: Union[MDAnalysisParser, PymatgenParser]) -> List[np.ndarray]:
         """
-        If more than one trajectory is given, then they are stacked to give the appearence that there are
+        If more than one trajectory is given, then they are stacked to give the appearance that there are
         additional atoms in the trajectory.
 
         :param u: Results from the parsing of each trajectory.
 
         :return: The stacked displacement list.
         """
         joint_disp_3d = []
@@ -268,15 +304,15 @@
         :return: Timestep values that have been sampled.
         """
         return self._diff.dt
 
     @property
     def dr(self) -> List['uravu.distribution.Distribution']:
         """
-        :return: A list of :py:class:`uravu.distribution.Distribution` objects that describe the euclidian
+        :return: A list of :py:class:`uravu.distribution.Distribution` objects that describe the Euclidean
             displacement at each :py:attr:`dt`.
         """
         return self._diff.euclidian_displacements
 
     @property
     def ngp_max(self) -> float:
         """
```

### Comparing `kinisi-0.6.5/kinisi/arrhenius.py` & `kinisi-0.7.0/kinisi/arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/kinisi/conductivity_analyzer.py` & `kinisi-0.7.0/kinisi/conductivity_analyzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,14 +87,49 @@
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         cond_anal = super()._from_pymatgen(trajectory, parser_params, dtype=dtype)
         cond_anal._diff = diffusion.MSCDBootstrap(cond_anal._delta_t, cond_anal._disp_3d, ionic_charge, cond_anal._n_o,
                                                   **bootstrap_params)
         return cond_anal
+    
+
+    @classmethod
+    def from_ase(cls,
+                      trajectory: List[Union['ase.atoms.Atoms',
+                                             List['ase.atom.Atoms']]],
+                      parser_params: dict,
+                      dtype: str = None,
+                      bootstrap_params: dict = None,
+                      ionic_charge: Union[np.ndarray, int] = 1):
+        """
+        Create a :py:class:`ConductivityAnalyzer` object from a list or nested list of
+        :py:class:`ase.Atoms` objects.
+
+        :param trajectory: The list or nested list of structures to be analysed.
+        :param parser_params: The parameters for the :py:class:`kinisi.parser.ASEParser` object. See the
+            appropriate documentation for more guidance on this dictionary.
+        :param dtype: If :py:attr:`trajectory` is a list of :py:class:`ase.Atoms` objects,
+            this should be :py:attr:`None`. However, if a list of lists is passed, then it is necessary to identify if
+            these constitute a series of :py:attr:`consecutive` trajectories or a series of :py:attr:`identical`
+            starting points with different random seeds, in which case the `dtype` should be either
+            :py:attr:`consecutive` or :py:attr:`identical`.
+        :param bootstrap_params: The parameters for the :py:class:`kinisi.diffusion.MSDBootstrap` object. See the
+            appropriate documentation for more guidance on this. Optional, default is the default bootstrap parameters.
+        :param ionic_charge: The charge on the mobile ions, either an array with a value for each ion or a scalar
+            if all values are the same. Optional, default is :py:attr:`1`.
+
+        :return: Relevant :py:class:`ConductivityAnalyzer` object.
+        """
+        if bootstrap_params is None:
+            bootstrap_params = {}
+        cond_anal = super()._from_ase(trajectory, parser_params, dtype=dtype)
+        cond_anal._diff = diffusion.MSCDBootstrap(cond_anal._delta_t, cond_anal._disp_3d, ionic_charge, cond_anal._n_o,
+                                                  **bootstrap_params)
+        return cond_anal
 
     @classmethod
     def from_Xdatcar(cls,
                      trajectory: Union['pymatgen.io.vasp.outputs.Xdatcar', List['pymatgen.io.vasp.outputs.Xdatcar']],
                      parser_params: dict,
                      dtype: str = None,
                      bootstrap_params: dict = None,
@@ -184,26 +219,28 @@
         if bootstrap_params is None:
             bootstrap_params = {}
         cond_anal = super()._from_universe(trajectory, parser_params, dtype=dtype)
         cond_anal._diff = diffusion.MSCDBootstrap(cond_anal._delta_t, cond_anal._disp_3d, ionic_charge, cond_anal._n_o,
                                                   **bootstrap_params)
         return cond_anal
 
-    def conductivity(self, temperature: float, conductivity_params: Union[dict, None] = None):
+    def conductivity(self, start_dt: float, temperature: float, conductivity_params: Union[dict, None] = None):
         """
         Calculate the jump diffusion coefficicent using the bootstrap-GLS methodology.
 
+        :param start_dt: The starting time for the analysis to find the diffusion coefficient.
+            This should be the start of the diffusive regime in the simulation.
         :param temperature: Simulation temperature in Kelvin
         :param conductivity_params: The parameters for the :py:class:`kinisi.diffusion.MSCDBootstrap` object.
             See the appropriate documentation for more guidance on this. Optional, default is the default
             bootstrap parameters
         """
         if conductivity_params is None:
             conductivity_params = {}
-        self._diff.conductivity(temperature, self._volume, **conductivity_params)
+        self._diff.conductivity(start_dt, temperature, self._volume, **conductivity_params)
 
     @property
     def mscd(self) -> np.ndarray:
         """
         :return: MSCD for the input trajectories. Note that this is the bootstrap sampled value, not the numerical
             average from the data.
         """
```

### Comparing `kinisi-0.6.5/kinisi/diffusion.py` & `kinisi-0.7.0/kinisi/diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -290,70 +290,64 @@
         :return: Value of non-Gaussian parameter.
         """
         top = np.mean(d_squared * d_squared) * 3
         bottom = np.square(np.mean(d_squared)) * 5
         return top / bottom - 1
 
     def bootstrap_GLS(self,
-                      use_ngp: bool = False,
-                      dt_skip: float = 0,
+                      start_dt: float,
                       fit_intercept: bool = True,
                       n_samples: int = 1000,
                       n_walkers: int = 32,
                       n_burn: int = 500,
                       thin: int = 10,
                       progress: bool = True,
                       random_state: np.random.mtrand.RandomState = None):
         """
         Use the covariance matrix estimated from the resampled values to estimate the gradient and intercept
         using a generalised least squares approach.
 
-        :param use_ngp: Should the ngp max be used as the starting point for the diffusion fitting. Optional,
-            default is :py:attr:`False`.
-        :param dt_skip: Values of :py:attr:`dt` that should be skipped, i.e. where the atoms are not diffusing.
-            Note that if :py:attr:`use_ngp` is :py:attr:`True` this will be ignored. Optional, defaults
-            to :py:attr:`0`.
+        :param start_dt: The starting time for the analysis to find the diffusion coefficient.
+            This should be the start of the diffusive regime in the simulation.
         :param fit_intercept: Should the intercept of the diffusion relationship be fit. Optional, default
             is :py:attr:`True`.
         :param n_samples: Number of samples of the Gaussian process to perform. Optional, default is :py:attr:`1000`.
         :param n_walkers: Number of MCMC walkers to use. Optional, default is :py:attr:`32`.
         :param n_burn: Number of burn in samples (these allow the sampling to settle). Optional, default
             is :py:attr:`500`.
         :param thin: Use only every :py:attr:`thin` samples for the MCMC sampler. Optional, default is :py:attr:`10`.
         :param progress: Show tqdm progress for sampling. Optional, default is :py:attr:`True`.
         :param random_state: A :py:attr:`RandomState` object to be used to ensure reproducibility. Optional,
             default is :py:attr:`None`.
         """
         if random_state is not None:
             np.random.seed(random_state.get_state()[1][1])
 
-        max_ngp = np.argwhere(self._dt > dt_skip)[0][0]
-        if use_ngp:
-            max_ngp = np.argmax(self._ngp)
+        diff_regime = np.argwhere(self._dt >= start_dt)[0][0]
 
-        self._covariance_matrix = self.generate_covariance_matrix(max_ngp)
+        self._covariance_matrix = self.generate_covariance_matrix(diff_regime)
 
         _, logdet = np.linalg.slogdet(self._covariance_matrix)
-        logdet += np.log(2 * np.pi) * self._n[max_ngp:].size
+        logdet += np.log(2 * np.pi) * self._n[diff_regime:].size
         inv = pinvh(self._covariance_matrix)
 
         def log_likelihood(theta: np.ndarray) -> float:
             """
             Get the log likelihood for multivariate normal distribution.
             :param theta: Value of the gradient and intercept of the straight line.
             :return: Log-likelihood value.
             """
             if theta[0] < 0:
                 return -np.inf
-            model = _straight_line(self._dt[max_ngp:], *theta)
-            diff = (model - self._n[max_ngp:])
+            model = _straight_line(self._dt[diff_regime:], *theta)
+            diff = (model - self._n[diff_regime:])
             logl = -0.5 * (logdet + np.matmul(diff.T, np.matmul(inv, diff)))
             return logl
 
-        ols = linregress(self._dt[max_ngp:], self._n[max_ngp:])
+        ols = linregress(self._dt[diff_regime:], self._n[diff_regime:])
         slope = ols.slope
         intercept = 1e-20
         if slope < 0:
             slope = 1e-20
 
         def nll(*args) -> float:
             """
@@ -375,85 +369,92 @@
         sampler.run_mcmc(pos, n_samples + n_burn, progress=progress, progress_kwargs={'desc': "Likelihood Sampling"})
         self.flatchain = sampler.get_chain(flat=True, thin=thin, discard=n_burn)
         self.gradient = Distribution(self.flatchain[:, 0])
         self._intercept = None
         if fit_intercept:
             self._intercept = Distribution(self.flatchain[:, 1])
 
-    def generate_covariance_matrix(self, max_ngp: int):
+    def generate_covariance_matrix(self, diff_regime: int):
         """
         Generate the covariance matrix, including the modelling and finding the closest matrix
         that is positive definite.
 
-        :param max_ngp: The index of the maximum of the non-Gaussian parameter or the point
-            where the analysis should begin.
+        :param diff_regime: The index of the point where the analysis should begin.
         :return: Modelled covariance matrix that is positive definite.
         """
 
         def _model_variance(dt: np.ndarray, a: float) -> np.ndarray:
             """
             Determine the model variance, based on a quadratic relationship with the number of
             independent samples as a divisor.
 
             :param dt: Timestep value
             :param a: Quadratic coefficient
             :return: Model variances
             """
-            return a / self._n_o[max_ngp:] * dt**2
+            return a / self._n_o[diff_regime:] * dt**2
 
-        self._popt, _ = curve_fit(_model_variance, self.dt[max_ngp:], self._v[max_ngp:])
-        self._model_v = _model_variance(self.dt[max_ngp:], *self._popt)
-        self._covariance_matrix = _populate_covariance_matrix(self._model_v, self._n_o[max_ngp:])
+        self._popt, _ = curve_fit(_model_variance, self.dt[diff_regime:], self._v[diff_regime:])
+        self._model_v = _model_variance(self.dt[diff_regime:], *self._popt)
+        self._covariance_matrix = _populate_covariance_matrix(self._model_v, self._n_o[diff_regime:])
         self._npd_covariance_matrix = self._covariance_matrix
         return find_nearest_positive_definite(self._covariance_matrix)
 
-    def diffusion(self, **kwargs):
+    def diffusion(self, start_dt: float, **kwargs):
         """
         Use the bootstrap-GLS method to determine the diffusivity for the system. Keyword arguments will be
         passed of the :py:func:`bootstrap_GLS` method.
+
+        :param start_dt: The starting time for the analysis to find the diffusion coefficient.
+            This should be the start of the diffusive regime in the simulation.
         """
-        self.bootstrap_GLS(**kwargs)
+        self.bootstrap_GLS(start_dt, **kwargs)
         self._diffusion_coefficient = Distribution(self.gradient.samples / (2e4 * self.dims))
 
     @property
     def D(self) -> Union[Distribution, None]:
         """
         An alias for the diffusion coefficient Distribution.
 
         :return: Diffusion coefficient, with units of cm:sup:`2`s:sup:`-1`.
         """
         return self._diffusion_coefficient
 
-    def jump_diffusion(self, **kwargs):
+    def jump_diffusion(self, start_dt: float, **kwargs):
         """
         Use the bootstrap-GLS method to determine the jump diffusivity for the system. Keyword arguments
         will be passed of the :py:func:`bootstrap_GLS` method.
+
+        :param start_dt: The starting time for the analysis to find the diffusion coefficient.
+            This should be the start of the diffusive regime in the simulation.
         """
-        self.bootstrap_GLS(**kwargs)
+        self.bootstrap_GLS(start_dt, **kwargs)
         self._jump_diffusion_coefficient = Distribution(self.gradient.samples /
                                                         (2e4 * self.dims * self._displacements[0].shape[0]))
 
     @property
     def D_J(self) -> Union[Distribution, None]:
         """
         Alias for the jump diffusion coefficient Distribution.
 
         :return: Jump diffusion coefficient, with units of cm:sup:`2`s:sup:`-1`.
         """
         return self._jump_diffusion_coefficient
 
-    def conductivity(self, temperature: float, volume: float, **kwargs):
+    def conductivity(self, start_dt: float, temperature: float, volume: float, **kwargs):
         """
         Use the bootstrap-GLS method to determine the ionic conductivity for the system, in units of mScm:sup:`-1`.
         Keyword arguments will be passed of the :py:func:`bootstrap_GLS` method.
 
+        :param start_dt: The starting time for the analysis to find the diffusion coefficient.
+            This should be the start of the diffusive regime in the simulation.
         :param temperature: System temperature, in Kelvin.
         :param volume: System volume, in Å^{3}.
         """
-        self.bootstrap_GLS(**kwargs)
+        self.bootstrap_GLS(start_dt, **kwargs)
         volume = volume * 1e-24  # cm^3
         D = self.gradient.samples / (2e4 * self.dims)  # cm^2s^-1
         conversion = 1000 / (volume * const.N_A) * (const.N_A * const.e)**2 / (const.R * temperature)
         self._sigma = Distribution(D * conversion)
 
     @property
     def sigma(self) -> Union[Distribution, None]:
```

### Comparing `kinisi-0.6.5/kinisi/diffusion_analyzer.py` & `kinisi-0.7.0/kinisi/diffusion_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,44 @@
         :return: Relevant :py:class:`DiffusionAnalyzer` object.
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         diff = super()._from_pymatgen(trajectory, parser_params, dtype=dtype)
         diff._diff = diffusion.MSDBootstrap(diff._delta_t, diff._disp_3d, diff._n_o, **bootstrap_params)
         return diff
+    
+    @classmethod
+    def from_ase(cls,
+                    trajectory: List[Union['ase.atoms.Atoms', List['ase.atoms.Atoms']]],
+                    parser_params: dict,
+                    dtype: str = None,
+                    bootstrap_params: dict = None):
+        """
+        Create a :py:class:`DiffusionAnalyzer` object from a list or nested list of
+        :py:class:`ase.atoms.Atoms` objects.
+
+        :param trajectory: The list or nested list of structures to be analysed.
+        :dtype trajectory: List[Union['ase.atoms.Atoms', List['ase.atoms.Atoms']]]
+        :param parser_params: The parameters for the :py:class:`kinisi.parser.ASEParser` object. See the
+            appropriate documentation for more guidance on this dictionary.
+        :param dtype: If :py:attr:`trajectory` is a list of :py:class:`ase.atoms.Atoms` objects,
+            this should be :py:attr:`None`. However, if a list of lists is passed, then it is necessary to identify if
+            these constitute a series of :py:attr:`consecutive` trajectories or a series of :py:attr:`identical`
+            starting points with different random seeds, in which case the `dtype` should be either
+            :py:attr:`consecutive` or :py:attr:`identical`.
+        :param bootstrap_params: The parameters for the :py:class:`kinisi.diffusion.MSDBootstrap` object. See the
+            appropriate documentation for more guidance on this. Optional, default is the default bootstrap parameters.
+
+        :return: Relevant :py:class:`DiffusionAnalyzer` object.
+        """
+        if bootstrap_params is None:
+            bootstrap_params = {}
+        diff = super()._from_ase(trajectory, parser_params, dtype=dtype)
+        diff._diff = diffusion.MSDBootstrap(diff._delta_t, diff._disp_3d, diff._n_o, **bootstrap_params)
+        return diff
 
     @classmethod
     def from_Xdatcar(cls,
                      trajectory: Union['pymatgen.io.vasp.outputs.Xdatcar', List['pymatgen.io.vasp.outputs.Xdatcar']],
                      parser_params: dict,
                      dtype: str = None,
                      bootstrap_params: dict = None):
@@ -167,25 +197,27 @@
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         diff = super()._from_universe(trajectory, parser_params, dtype=dtype)
         diff._diff = diffusion.MSDBootstrap(diff._delta_t, diff._disp_3d, diff._n_o, **bootstrap_params)
         return diff
 
-    def diffusion(self, diffusion_params: Union[dict, None] = None):
+    def diffusion(self, start_dt: float, diffusion_params: Union[dict, None] = None):
         """
         Calculate the diffusion coefficicent using the bootstrap-GLS methodology.
 
+        :param start_dt: The starting time for the analysis to find the diffusion coefficient.
+            This should be the start of the diffusive regime in the simulation.
         :param diffusion_params: The parameters for the :py:class:`kinisi.diffusion.MSDBootstrap` object.
             See the appropriate documentation for more guidance on this. Optional, default is the default bootstrap
             parameters.
         """
         if diffusion_params is None:
             diffusion_params = {}
-        self._diff.diffusion(**diffusion_params)
+        self._diff.diffusion(start_dt, **diffusion_params)
 
     @property
     def msd(self) -> np.ndarray:
         """
         :return: MSD for the input trajectories. Note that this is the bootstrap sampled MSD, not the numerical
         average from the data.
         """
```

### Comparing `kinisi-0.6.5/kinisi/jump_diffusion_analyzer.py` & `kinisi-0.7.0/kinisi/jump_diffusion_analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,44 @@
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         jdiff_anal = super()._from_pymatgen(trajectory, parser_params, dtype=dtype)
         jdiff_anal._diff = diffusion.MSTDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
                                                    **bootstrap_params)
         return jdiff_anal
+    
+    @classmethod
+    def from_ase(cls,
+                    trajectory: List[Union['ase.atoms.Atoms', List['ase.atoms.Atoms']]],
+                    parser_params: dict,
+                    dtype: str = None,
+                    bootstrap_params: dict = None):
+        """
+        Create a :py:class:`JumpDiffusionAnalyzer` object from a list or nested list of
+        :py:class:`ase.atoms.Atoms` objects.
+
+        :param trajectory: The list or nested list of structures to be analysed.
+        :param parser_params: The parameters for the :py:class:`kinisi.parser.AseParser` object. See the
+            appropriate documentation for more guidance on this dictionary.
+        :param dtype: If :py:attr:`trajectory` is a list of :py:class:`ase.atoms.Atoms` objects,
+            this should be :py:attr:`None`. However, if a list of lists is passed, then it is necessary to identify if
+            these constitute a series of :py:attr:`consecutive` trajectories or a series of :py:attr:`identical`
+            starting points with different random seeds, in which case the `dtype` should be either
+            :py:attr:`consecutive` or :py:attr:`identical`.
+        :param bootstrap_params: The parameters for the :py:class:`kinisi.diffusion.MSDBootstrap` object. See the
+            appropriate documentation for more guidance on this. Optional, default is the default bootstrap parameters.
+        
+        :return: Relevant :py:class:`JumpDiffusionAnalyzer` object.
+        """
+        if bootstrap_params is None:
+            bootstrap_params = {}
+        jdiff_anal = super()._from_ase(trajectory, parser_params, dtype=dtype)
+        jdiff_anal._diff = diffusion.MSTDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
+                                                    **bootstrap_params)
+        return jdiff_anal
 
     @classmethod
     def from_Xdatcar(cls,
                      trajectory: Union['pymatgen.io.vasp.outputs.Xdatcar', List['pymatgen.io.vasp.outputs.Xdatcar']],
                      parser_params: dict,
                      dtype: str = None,
                      bootstrap_params: dict = None):
@@ -170,25 +200,27 @@
         if bootstrap_params is None:
             bootstrap_params = {}
         jdiff_anal = super()._from_universe(trajectory, parser_params, dtype=dtype)
         jdiff_anal._diff = diffusion.MSTDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
                                                    **bootstrap_params)
         return jdiff_anal
 
-    def jump_diffusion(self, jump_diffusion_params: Union[dict, None] = None):
+    def jump_diffusion(self, start_dt: float, jump_diffusion_params: Union[dict, None] = None):
         """
         Calculate the jump diffusion coefficicent using the bootstrap-GLS methodology.
 
+        :param start_dt: The starting time for the analysis to find the diffusion coefficient.
+            This should be the start of the diffusive regime in the simulation.
         :param ump_diffusion_params: The parameters for the :py:class:`kinisi.diffusion.MSTDBootstrap`
             object. See the appropriate documentation for more guidance on this. Optional, default is the
             default bootstrap parameters.
         """
         if jump_diffusion_params is None:
             jump_diffusion_params = {}
-        self._diff.jump_diffusion(**jump_diffusion_params)
+        self._diff.jump_diffusion(start_dt, **jump_diffusion_params)
 
     @property
     def mstd(self) -> np.ndarray:
         """
         :return: MSTD for the input trajectories. Note that this is the bootstrap sampled MSD, not the numerical
             average from the data.
         """
```

### Comparing `kinisi-0.6.5/kinisi/matrix.py` & `kinisi-0.7.0/kinisi/matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/kinisi/parser.py` & `kinisi-0.7.0/kinisi/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -203,14 +203,136 @@
             else:
                 raise ValueError(f"The sampling option of {self.sampling} is unrecognized, "
                                  "please use 'multi-origin' or 'single-origin'.")
             # n_samples = np.append(n_samples, np.multiply(*disp[:, ::timestep].shape[:2]))
             n_samples = np.append(n_samples, disp.shape[0] * timesteps[-1] / timestep)
         return delta_t, disp_3d, n_samples
 
+class ASEParser(Parser):
+    """
+    A parser for ASE Atoms objects
+    
+    :param atoms: Atoms ordered in sequence of run.
+    :param specie: symbol to calculate diffusivity for as a String, e.g. :py:attr:`'Li'`.
+    :param time_step: Time step, in picoseconds, between steps in trajectory.
+    :param step_skip: Sampling frequency of the trajectory (time_step is multiplied by this number to get the real
+        time between output from the simulation file).
+    :param sub_sample_traj: Multiple of the :py:attr:`time_step` to sub sample at. Optional, defaults
+        to :py:attr:`1` where all timesteps are used.
+    :param min_dt: Minimum timestep to be evaluated, in the simulation units. Optional, defaults to the
+        produce of :py:attr:`time_step` and :py:attr:`step_skip`.
+    :param max_dt: Maximum timestep to be evaluated, in the simulation units. Optional, defaults to the
+        length of the simulation.
+    :param n_steps: Number of steps to be used in the timestep function. Optional, defaults to :py:attr:`100`
+        unless this is fewer than the total number of steps in the trajectory when it defaults to this number.
+    :param spacing: The spacing of the steps that define the timestep, can be either :py:attr:`'linear'` or
+        :py:attr:`'logarithmic'`. If :py:attr:`'logarithmic'` the number of steps will be less than or equal
+        to that in the :py:attr:`n_steps` argument, such that all values are unique. Optional, defaults to
+        :py:attr:`linear`.
+    :param sampling: The ways that the time-windows are sampled. The options are :py:attr:`'single-origin'`
+        or :py:attr:`'multi-origin'` with the former resulting in only one observation per atom per
+        time-window and the latter giving the maximum number of origins without sampling overlapping
+        trajectories. Optional, defaults to :py:attr:`'multi-origin'`.
+    :param memory_limit: Upper limit in the amount of computer memory that the displacements can occupy in
+        gigabytes (GB). Optional, defaults to :py:attr:`8.`.
+    :param progress: Print progress bars to screen. Optional, defaults to :py:attr:`True`.
+    """
+    def __init__(self, 
+                 atoms: List["ase.atoms.Atoms"],
+                 specie: str,
+                 time_step: float,
+                 step_skip: int,
+                 sub_sample_traj: int = 1,
+                 min_dt: float = None,
+                 max_dt: float = None,
+                 n_steps: int = 100,
+                 spacing: str = 'linear',
+                 sampling: str = 'multi-origin',
+                 memory_limit: float = 8.,
+                 progress: bool = True):
+        
+            structure, coords, latt = self.get_structure_coords_latt(atoms, sub_sample_traj, progress)
+            indices = self.get_indices(structure, specie)
+
+            super().__init__(self.get_disp(coords, latt),
+                         indices[0], 
+                         indices[1], 
+                         time_step, 
+                         step_skip, 
+                         min_dt, 
+                         max_dt, 
+                         n_steps, 
+                         spacing, 
+                         sampling, 
+                         memory_limit, 
+                         progress)
+            self._volume = structure.get_volume()
+            
+        
+    @staticmethod
+    def get_structure_coords_latt(
+                atoms: List["ase.atoms.Atoms"],
+                sub_sample_traj: int = 1,
+                progress: bool = True) -> Tuple["ase.atoms.Atoms", List[np.ndarray], List[np.ndarray]]:
+            """
+            Obtain the initial structure and displacement from a :py:attr:`list`
+            of :py:class`pymatgen.core.structure.Structure`.
+
+            :param structures: Structures ordered in sequence of run.
+            :param sub_sample_traj: Multiple of the :py:attr:`time_step` to sub sample at.
+                Optional, default is :py:attr:`1`.
+            :param progress: Print progress bars to screen. Optional, defaults to :py:attr:`True`.
+
+            :return: Tuple containing: initial structure, fractional coordinates for all atoms,
+                and lattice descriptions.
+            """
+            coords, latt = [], []
+            first = True
+            if progress:
+                iterator = tqdm(atoms[::sub_sample_traj], desc='Reading Trajectory')
+            else:
+                iterator = atoms[::sub_sample_traj]
+            for struct in iterator:
+                if first:
+                    structure = struct
+                    first = False
+                scaled_positions = struct.get_scaled_positions()
+                coords.append(np.array(scaled_positions)[:, None])
+                latt.append(struct.cell[:])
+            
+            coords.insert(0, coords[0])
+            latt.insert(0, latt[0])
+            return structure, coords, latt
+    
+    @staticmethod
+    def get_indices(
+        structure: "ase.atoms.Atoms",
+        specie: "str"
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Determine framework and non-framework indices for a :py:mod:`pymatgen` compatible file.
+
+        :param structure: Initial structure.
+        :param specie: Specie to calculate diffusivity for as a String, e.g. :py:attr:`'Li'`.
+
+        :returns: Tuple containing: indices for the atoms in the trajectory used in the calculation of the diffusion
+            and indices of framework atoms.
+        """
+        indices = []
+        framework_indices = []
+        if not isinstance(specie, List):
+            specie = [specie]
+        for i, site in enumerate(structure):
+            if site.symbol in specie:
+                indices.append(i)
+            else:
+                framework_indices.append(i)
+        if len(indices) == 0:
+            raise ValueError("There are no species selected to calculate the mean-squared displacement of.")
+        return indices, framework_indices
 
 class PymatgenParser(Parser):
     """
     A parser for pymatgen structures.
 
     :param structures: Structures ordered in sequence of run.
     :param specie: Specie to calculate diffusivity for as a String, e.g. :py:attr:`'Li'`.
@@ -295,14 +417,15 @@
             iterator = structures[::sub_sample_traj]
         for struct in iterator:
             if first:
                 structure = struct
                 first = False
             coords.append(np.array(struct.frac_coords)[:, None])
             latt.append(struct.lattice.matrix)
+
         coords.insert(0, coords[0])
         latt.insert(0, latt[0])
         return structure, coords, latt
 
     @staticmethod
     def get_indices(
         structure: "pymatgen.core.structure.Structure",
```

### Comparing `kinisi-0.6.5/kinisi/tests/test_analyze.py` & `kinisi-0.7.0/kinisi/tests/test_analyze.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,81 @@
 import os
 import warnings
 import unittest
 import numpy as np
 from numpy.testing import assert_almost_equal, assert_equal
 from pymatgen.io.vasp import Xdatcar
 import MDAnalysis as mda
+from ase.io import Trajectory
 from uravu.distribution import Distribution
 import kinisi
 from kinisi.analyze import DiffusionAnalyzer, JumpDiffusionAnalyzer, ConductivityAnalyzer
 from kinisi.analyzer import Analyzer, _flatten_list
 
 file_path = os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_XDATCAR.gz')
 xd = Xdatcar(file_path)
 da_params = {'specie': 'Li', 'time_step': 2.0, 'step_skip': 50}
 md = mda.Universe(os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_LAMMPS.data'),
                   os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_LAMMPS.dcd'),
                   format='LAMMPS')
 db_params = {'specie': '1', 'time_step': 0.005, 'step_skip': 250}
+ase_file_path = os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_ase.traj')
+traj = Trajectory(ase_file_path, 'r')
+dc_params = {'specie': 'Li', 'time_step': 1.0 * 1e-3, 'step_skip': 1}
+
 
 
 class TestAnalyzer(unittest.TestCase):
     """
     Tests for the Analyzer base class.
     """
 
+    @classmethod
+    def tearDownClass(cls):
+        test_files = ['test_save.hdf', 'test_load.hdf']
+        for test_file in test_files:
+            if os.path.exists(test_file):
+                os.remove(test_file)
+    
+    def test_save(self):
+        a = Analyzer._from_pymatgen(xd.structures, parser_params=da_params)
+        filename = "test_save"
+        a.save(filename)
+        assert os.path.exists(filename + ".hdf")
+
+    def tearDown(self):
+        for filename in ["test_save", "test_load"]:
+            if os.path.exists(filename + ".hdf"):
+                os.remove(filename + ".hdf")
+
+    def test_to_dict(self):
+        a = Analyzer._from_pymatgen(xd.structures, parser_params=da_params)
+        dictionary = a.to_dict()
+        assert isinstance(dictionary, dict)
+        assert set(dictionary.keys()) == set(['delta_t', 'disp_3d', 'n_o', 'volume'])
+
+    def test_from_dict(self):
+        a = Analyzer._from_pymatgen(xd.structures, parser_params=da_params)
+        dictionary = a.to_dict()
+        b = Analyzer.from_dict(dictionary)
+        assert_equal(a._delta_t, b._delta_t)
+        for i, d in enumerate(a._disp_3d):
+            assert_equal(d, b._disp_3d[i])
+        assert a._volume == b._volume
+
+    def test_load(self):
+        a = Analyzer._from_pymatgen(xd.structures, parser_params=da_params)
+        filename = "test_load"
+        a.save(filename)
+        loaded = Analyzer.load(filename)
+        assert_equal(a._delta_t, loaded._delta_t)
+        for i, d in enumerate(a._disp_3d):
+            assert_equal(d, loaded._disp_3d[i])
+        assert a._volume == loaded._volume
+
     def test_dict_roundtrip(self):
         a = Analyzer._from_pymatgen(xd.structures, parser_params=da_params)
         b = Analyzer.from_dict(a.to_dict())
         assert_equal(a._delta_t, b._delta_t)
         for i, d in enumerate(a._disp_3d):
             assert_equal(d, b._disp_3d[i])
         assert a._volume == b._volume
@@ -127,14 +175,30 @@
         a = Analyzer._from_universe([md, md], parser_params=db_params, dtype='identical')
         assert a._delta_t.size == 100
         assert_almost_equal(a._delta_t.max(), 250.)
         assert len(a._disp_3d) == 100
         assert a._disp_3d[0].shape == (408, 200, 3)
         assert a._disp_3d[-1].shape == (408, 1, 3)
 
+    def test_ase(self):
+        a = Analyzer._from_ase(traj, parser_params=dc_params)
+        assert a._delta_t.size == 100
+        assert_almost_equal(a._delta_t.max(), 0.2)
+        assert len(a._disp_3d) == 100
+        assert a._disp_3d[0].shape == (180, 200, 3)
+        assert a._disp_3d[-1].shape == (180, 1, 3)
+
+    def test_identical_ase(self):
+        a = Analyzer._from_ase([traj, traj], parser_params=dc_params, dtype='identical')
+        assert a._delta_t.size == 100
+        assert_almost_equal(a._delta_t.max(), 0.2)
+        assert len(a._disp_3d) == 100
+        assert a._disp_3d[0].shape == (360, 200, 3)
+        assert a._disp_3d[-1].shape == (360, 1, 3)
+
     def test_list_bad_input(self):
         with self.assertRaises(ValueError):
             _ = Analyzer._from_file([file_path, file_path], parser_params=da_params, dtype='consecutie')
 
     def test_list_bad_mda(self):
         with self.assertRaises(ValueError):
             _ = Analyzer._from_universe(file_path, parser_params=db_params, dtype='consecutie')
@@ -163,30 +227,30 @@
                                                 parser_params=da_params,
                                                 bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.msd, a._diff.n)
             assert_almost_equal(a.msd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
-            a.diffusion()
+            a.diffusion(0)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D, Distribution)
             assert a.flatchain.shape == (3200, 2)
 
     def test_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as _:
             a = DiffusionAnalyzer.from_pymatgen(xd.structures,
                                                 parser_params=da_params,
                                                 bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.msd, a._diff.n)
             assert_almost_equal(a.msd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
-            a.diffusion()
+            a.diffusion(0)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D, Distribution)
             assert a.flatchain.shape == (3200, 2)
             b = DiffusionAnalyzer.from_dict(a.to_dict())
             assert_equal(a.dt, b.dt)
             assert_equal(a.msd, b.msd)
             assert_equal(a.msd_std, b.msd_std)
@@ -220,30 +284,30 @@
                                                     parser_params=da_params,
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.mstd, a._diff.n)
             assert_almost_equal(a.mstd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
-            a.jump_diffusion()
+            a.jump_diffusion(0)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D_J, Distribution)
             assert a.flatchain.shape == (3200, 2)
 
     def test_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as w:
             a = JumpDiffusionAnalyzer.from_pymatgen(xd.structures,
                                                     parser_params=da_params,
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.mstd, a._diff.n)
             assert_almost_equal(a.mstd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
-            a.jump_diffusion()
+            a.jump_diffusion(0)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D_J, Distribution)
             assert a.flatchain.shape == (3200, 2)
             b = JumpDiffusionAnalyzer.from_dict(a.to_dict())
             assert_equal(a.dt, b.dt)
             assert_equal(a.mstd, b.mstd)
             assert_equal(a.mstd_std, b.mstd_std)
@@ -279,30 +343,30 @@
                                                    bootstrap_params={'random_state': np.random.RandomState(0)},
                                                    ionic_charge=1)
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.mscd, a._diff.n)
             assert_almost_equal(a.mscd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
-            a.conductivity(100)
+            a.conductivity(0, temperature=100)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.sigma, Distribution)
             assert a.flatchain.shape == (3200, 2)
 
     def test_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as w:
             a = ConductivityAnalyzer.from_pymatgen(xd.structures,
                                                    parser_params=da_params,
                                                    bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.mscd, a._diff.n)
             assert_almost_equal(a.mscd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
-            a.conductivity(100)
+            a.conductivity(0, temperature=100)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.sigma, Distribution)
             assert a.flatchain.shape == (3200, 2)
             b = ConductivityAnalyzer.from_dict(a.to_dict())
             assert_equal(a.dt, b.dt)
             assert_equal(a.mscd, b.mscd)
             assert_equal(a.mscd_std, b.mscd_std)
```

### Comparing `kinisi-0.6.5/kinisi/tests/test_arrhenius.py` & `kinisi-0.7.0/kinisi/tests/test_arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/kinisi/tests/test_diffusion.py` & `kinisi-0.7.0/kinisi/tests/test_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
     def test_bootstrap_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             a = MSDBootstrap(dt, disp_3d, n_o, random_state=np.random.RandomState(0))
-            a.diffusion()
+            a.diffusion(0)
             b = MSDBootstrap.from_dict(a.to_dict())
             for i, d in enumerate(disp_3d):
                 assert_almost_equal(a._displacements[i], b._displacements[i])
             assert_almost_equal(a._delta_t, b._delta_t)
             assert a._max_obs == b._max_obs
             assert_equal(a.n, b.n)
             assert_equal(a.s, b.s)
@@ -269,92 +269,92 @@
 
     def test_bootstrap(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.diffusion()
+            bs.diffusion(0)
             assert bs.covariance_matrix.shape == (10, 10)
             assert isinstance(bs._diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._diffusion_coefficient.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_dt_skip(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSDBootstrap(dt, disp_3d, n_o)
-            bs.diffusion(dt_skip=150)
+            bs.diffusion(150)
             assert bs.covariance_matrix.shape == (9, 9)
             assert isinstance(bs._diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._diffusion_coefficient.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_use_ngp(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(200, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 190)
             bs = MSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.diffusion(use_ngp=True)
+            bs.diffusion(dt[bs.ngp.argmax()])
             assert bs.covariance_matrix.shape == (190 - np.argmax(bs.ngp), 190 - np.argmax(bs.ngp))
             assert isinstance(bs._diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._diffusion_coefficient.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_fit_intercept(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.diffusion(n_samples=500, fit_intercept=False)
+            bs.diffusion(0, n_samples=500, fit_intercept=False)
             assert bs.covariance_matrix.shape == (10, 10)
             assert isinstance(bs._diffusion_coefficient, Distribution)
             assert bs._diffusion_coefficient.size == 1600
             assert bs.intercept is None
 
     def test_bootstrap_n_samples(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.diffusion(n_samples=100)
+            bs.diffusion(0, n_samples=100)
             assert bs.covariance_matrix.shape == (10, 10)
             assert isinstance(bs._diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._diffusion_coefficient.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_D(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.diffusion(n_samples=100)
+            bs.diffusion(0, n_samples=100)
             assert bs.covariance_matrix.shape == (10, 10)
             assert isinstance(bs._diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs.D.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_thin(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.diffusion(use_ngp=True, thin=1)
+            bs.diffusion(dt[bs.ngp.argmax()], thin=1)
             assert bs.covariance_matrix.shape == (10 - np.argmax(bs.ngp), 10 - np.argmax(bs.ngp))
             assert isinstance(bs._diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._diffusion_coefficient.size == 32000
             assert bs.intercept.size == 32000
 
     # Waiting on https://github.com/dfm/emcee/pull/376
@@ -486,79 +486,79 @@
 
     def test_bootstrap(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.jump_diffusion()
+            bs.jump_diffusion(0)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_use_ngp(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.jump_diffusion(use_ngp=True)
+            bs.jump_diffusion(dt[bs.ngp.argmax()])
             assert bs.covariance_matrix.shape == (5 - np.argmax(bs.ngp), 5 - np.argmax(bs.ngp))
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_fit_intercept(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.jump_diffusion(n_samples=500, fit_intercept=False)
+            bs.jump_diffusion(0, n_samples=500, fit_intercept=False)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert bs._jump_diffusion_coefficient.size == 1600
             assert bs.intercept is None
 
     def test_bootstrap_n_samples(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.jump_diffusion(n_samples=100)
+            bs.jump_diffusion(0, n_samples=100)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_D(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.jump_diffusion(n_samples=100)
+            bs.jump_diffusion(0, n_samples=100)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_thin(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(200, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 190)
             bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
-            bs.jump_diffusion(use_ngp=True, thin=1)
+            bs.jump_diffusion(dt[bs.ngp.argmax()], thin=1)
             assert bs.covariance_matrix.shape == (95 - np.argmax(bs.ngp), 95 - np.argmax(bs.ngp))
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 32000
             assert bs.intercept.size == 32000
 
     # Waiting on https://github.com/dfm/emcee/pull/376
@@ -693,79 +693,79 @@
 
     def test_bootstrap(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=RNG)
-            bs.conductivity(1, 10)
+            bs.conductivity(0, 1, 10)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs.sigma, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs.sigma.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_use_ngp(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(200, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 190)
             bs = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=RNG)
-            bs.conductivity(1, 10, use_ngp=True)
+            bs.conductivity(dt[bs.ngp.argmax()], 1, 10)
             assert bs.covariance_matrix.shape == (95 - np.argmax(bs.ngp), 95 - np.argmax(bs.ngp))
             assert isinstance(bs.sigma, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs.sigma.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_fit_intercept(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=RNG)
-            bs.conductivity(1, 10, n_samples=500, fit_intercept=False)
+            bs.conductivity(0, 1, 10, n_samples=500, fit_intercept=False)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs.sigma, Distribution)
             assert bs.sigma.size == 1600
             assert bs.intercept is None
 
     def test_bootstrap_n_samples(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=RNG)
-            bs.conductivity(1, 10, n_samples=100)
+            bs.conductivity(0, 1, 10, n_samples=100)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs.sigma, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs.sigma.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_D(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
             bs = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=RNG)
-            bs.conductivity(1, 10, n_samples=100)
+            bs.conductivity(0, 1, 10, n_samples=100)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs.sigma, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs.sigma.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_thin(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(200, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 190)
             bs = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=RNG)
-            bs.conductivity(1, 10, use_ngp=True, thin=1)
+            bs.conductivity(dt[bs.ngp.argmax()], 1, 10, thin=1)
             assert bs.covariance_matrix.shape == (95 - np.argmax(bs.ngp), 95 - np.argmax(bs.ngp))
             assert isinstance(bs.sigma, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs.sigma.size == 32000
             assert bs.intercept.size == 32000
 
     # Waiting on https://github.com/dfm/emcee/pull/376
```

### Comparing `kinisi-0.6.5/kinisi/tests/test_matrix.py` & `kinisi-0.7.0/kinisi/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/kinisi/tests/test_parser.py` & `kinisi-0.7.0/kinisi/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # pylint: disable=R0201
 
 import unittest
 import numpy as np
 import MDAnalysis as mda
 from numpy.testing import assert_almost_equal, assert_equal
 from pymatgen.io.vasp import Xdatcar
+from ase.io import Trajectory
 import os
 import kinisi
 from kinisi import parser
 
 dc = np.random.random(size=(100, 100, 3))
 indices = np.arange(0, 100, 1, dtype=int)
 time_step = 1.0
@@ -101,14 +102,23 @@
         xd = Xdatcar(os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_XDATCAR.gz'))
         da_params = {'specie': 'Li', 'time_step': 20.0, 'step_skip': 100}
         data = parser.PymatgenParser(xd.structures, **da_params)
         assert_almost_equal(data.time_step, 20.0)
         assert_almost_equal(data.step_skip, 100)
         assert_equal(data.indices, list(range(xd.natoms[0])))
 
+    def test_ase_init(self):
+        traj = Trajectory(os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_ase.traj'))
+        da_params = {'specie': 'Li', 'time_step': 1e-3, 'step_skip': 1}
+        data = parser.ASEParser(traj, **da_params)
+        assert_almost_equal(data.time_step, 1e-3)
+        assert_almost_equal(data.step_skip, 1)
+        assert_equal(data.indices, list(range(180)))
+        
+
     def test_mda_init(self):
         xd = mda.Universe(os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_LAMMPS.data'),
                           os.path.join(os.path.dirname(kinisi.__file__), 'tests/inputs/example_LAMMPS.dcd'),
                           format='LAMMPS')
         da_params = {'specie': '1', 'time_step': 0.005, 'step_skip': 250}
         data = parser.MDAnalysisParser(xd, **da_params)
         assert_almost_equal(data.time_step, 0.005)
```

### Comparing `kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.data` & `kinisi-0.7.0/kinisi/tests/inputs/example_LAMMPS.data`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.dcd` & `kinisi-0.7.0/kinisi/tests/inputs/example_LAMMPS.dcd`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/kinisi/tests/inputs/example_XDATCAR.gz` & `kinisi-0.7.0/kinisi/tests/inputs/example_XDATCAR.gz`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/LICENSE` & `kinisi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/README.md` & `kinisi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.5/pyproject.toml` & `kinisi-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 dev = [
     'pymatgen',
     'MDAnalysis',
     'coverage',
     'codeclimate-test-reporter',
     'yapf',
     'pytest',
-    'pytest-cov'
+    'pytest-cov',
+    'ase',
+    'h5py'
 ]
 docs = [
     'pymatgen',
     'MDAnalysis',
     'ipykernel',
     'nbsphinx',
     'corner',
```

### Comparing `kinisi-0.6.5/PKG-INFO` & `kinisi-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinisi
-Version: 0.6.5
+Version: 0.7.0
 Summary: Efficient estimation of diffusion processes from molecular dynamics.
 Project-URL: homepage, https://github.com/bjmorgan/kinisi
 Project-URL: documentation, https://kinisi.rtfd.io
 Author-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 Maintainer-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 License-Expression: MIT
 License-File: LICENSE
@@ -22,16 +22,18 @@
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.9.3
 Requires-Dist: tqdm
 Requires-Dist: uravu>=1.2.9
 Provides-Extra: dev
+Requires-Dist: ase; extra == 'dev'
 Requires-Dist: codeclimate-test-reporter; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
+Requires-Dist: h5py; extra == 'dev'
 Requires-Dist: mdanalysis; extra == 'dev'
 Requires-Dist: pymatgen; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: yapf; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: corner; extra == 'docs'
```

