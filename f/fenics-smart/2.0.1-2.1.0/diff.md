# Comparing `tmp/fenics-smart-2.0.1.tar.gz` & `tmp/fenics-smart-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-smart-2.0.1.tar", last modified: Mon May 15 07:44:03 2023, max compression
+gzip compressed data, was "fenics-smart-2.1.0.tar", last modified: Fri Jun  9 01:35:48 2023, max compression
```

## Comparing `fenics-smart-2.0.1.tar` & `fenics-smart-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/fenics_smart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 07:44:03.000000 fenics-smart-2.0.1/fenics_smart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/smart/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    85874 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    50721 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/model_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/smart/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:44:03.915598 fenics-smart-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/tests/test_species.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-15 07:43:45.000000 fenics-smart-2.0.1/tests/test_stubs_model_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:35:48.842111 fenics-smart-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-06-09 01:35:48.842111 fenics-smart-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:35:48.838111 fenics-smart-2.1.0/fenics_smart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-06-09 01:35:48.000000 fenics-smart-2.1.0/fenics_smart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 01:35:48.000000 fenics-smart-2.1.0/fenics_smart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:35:48.000000 fenics-smart-2.1.0/fenics_smart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-09 01:35:48.000000 fenics-smart-2.1.0/fenics_smart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 01:35:48.000000 fenics-smart-2.1.0/fenics_smart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:35:48.842111 fenics-smart-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:35:48.842111 fenics-smart-2.1.0/smart/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27558 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/mesh_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89606 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63943 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/model_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/smart/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:35:48.842111 fenics-smart-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-09 01:35:28.000000 fenics-smart-2.1.0/tests/test_species.py
```

### Comparing `fenics-smart-2.0.1/LICENSE` & `fenics-smart-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.0.1/PKG-INFO` & `fenics-smart-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.0.1
+Version: 2.1.0
 Summary: SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -62,87 +62,109 @@
         
 Project-URL: homepage, https://rangamanilabucsd.github.io/smart
 Project-URL: repository, https://github.com/RangamaniLabUCSD/smart
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: examples
 Provides-Extra: all
 License-File: LICENSE
 
-Spatial Modelling Algorithms for Reaction-Transport [systems|models|equations]
-==============================
-[//]: # (Badges)
+[![Test fenics_smart](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml)
 [![PyPI](https://img.shields.io/pypi/v/fenics-smart)](https://pypi.org/project/fenics-smart/)
-
-
-SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models.
-SMART is highly suited for building systems biology models and simulating them as deterministic partial differential equations `[PDEs]` in realistic geometries using the Finite Element Method `[FEM]` - the integration of additional physics such as electro-diffusion or stochasticity may come in future updates.
-Systems biology models are converted by SMART into the appropriate systems of reaction-diffusion PDEs with proper boundary conditions.
-[FEniCS](https://fenicsproject.org/) is a core dependency of SMART which handles the assembly of finite element matrices as well as solving the resultant linear algebra systems.
+[![Deploy static content to Pages](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml)
+[![pre-commit](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml)
+# Spatial Modeling Algorithms for Reaction-Transport [systems|models|equations]
+
+## Statement of Need
+
+*Spatial Modeling Algorithms for Reactions and Transport* (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation for spatially-varying reaction-transport processes.
+SMART is based on the [FEniCS finite element library](https://fenicsproject.org/), provides a symbolic representation
+framework for specifying reaction pathways, and supports large and irregular cell geometries in 2D and 3D.
 
 - Documentation: https://rangamanilabucsd.github.io/smart
 - Source code: https://github.com/RangamaniLabUCSD/smart
 
 
 ## Installation
 
-### !!! IMPORTANT !!!
-Although FEniCS is a core dependency, because it has many different versions (2019.1, development, FEniCSx, etc.), is quite large, and is complicated to build, it is not packaged with SMART by default. The recommended way to use SMART is to create a container from one of the official FEniCS docker images and to pip install SMART from within the container.
+### Using docker (recommended)
+The simplest way to use `fenics-smart` is to use the provided docker image. You can get this image by pulling it from the github registry
+```
+docker pull ghcr.io/rangamanilabucsd/smart:latest
+```
+It is also possible to pull a specific version by changing the tag, e.g
+```
+docker pull ghcr.io/rangamanilabucsd/smart:v2.0.1
+```
+will use version 2.0.1.
 
-```bash
-# create a container using DOLFIN built on ubuntu 22.04 with Python 3.10
-jgl:~$ docker run -ti --init ghcr.io/scientificcomputing/fenics-gmsh:2023-04-21
-# pip install smart from within the container
-root@jgl:~$ python3 -m pip install fenics-smart
+In order to start a container you can use the [`docker run`](https://docs.docker.com/engine/reference/commandline/run/) command. For example the command
 ```
+docker run --rm -v $(pwd):/home/shared -w /home/shared -ti ghcr.io/rangamanilabucsd/smart:latest
+```
+will run the latest version and share your current working directory with the container.
 
-### Dependencies
-* SMART uses [FEniCS](https://fenicsproject.org/) to assemble finite element matrices as well as solve the resultant linear algebra systems.
-* SMART uses [pandas](https://pandas.pydata.org/) as an intermediate data structure to help organize and process models.
-* SMART uses [Pint](https://pint.readthedocs.io/en/stable/) for unit tracking and conversions.
-* SMART uses [matplotlib](https://matplotlib.org/) to automatically generate plots of min/mean/max (integrated over space) concentrations over time, as well as plots showing solver convergence.
-* SMART uses [sympy](https://www.sympy.org/) to allow users to input custom reactions and also to determine the appopriate solution techniques (e.g. testing for non-linearities).
-* SMART uses [numpy](https://numpy.org/) and [scipy](https://www.scipy.org/) for general array manipulations and basic calculations.
-* SMART uses [tabulate](https://pypi.org/project/tabulate/) to make pretty ASCII tables.
-* SMART uses [termcolor](https://pypi.org/project/termcolor/) for pretty terminal output so that simulations are more satisfying to watch.
+### Using pip
+`fenics-smart` is also available on [pypi](https://pypi.org/project/fenics-smart/) and can be installed with
+```
+python3 -m pip install fenics-smart
+```
+However this requires FEniCS version 2019.2.0 or later to already be installed. Currently, FEniCS version 2019.2.0 needs to be built [from source](https://bitbucket.org/fenics-project/dolfin/src/master/) or use some of the [pre-built docker images](https://github.com/orgs/scientificcomputing/packages?repo_name=packages)
+
+## Example usage
+The SMART repository contains a number of examples in the `examples` directory which also run as continuous integration tests (see "Automated Tests" below):
+* [Example 1](https://rangamanilabucsd.github.io/smart/examples/example1/example1.html): Formation of Turing patterns in 2D reaction-diffusion (rectangular domain)
+* [Example 2](https://rangamanilabucsd.github.io/smart/examples/example2/example2.html): Simple cell signaling model in 2D (ellipse)
+* [Example 3](https://rangamanilabucsd.github.io/smart/examples/example3/example3.html): Model of protein phosphorylation and diffusion in 3D (sphere)
+* [Example 4](https://rangamanilabucsd.github.io/smart/examples/example4/example4.html): Model of second messenger reaction-diffusion in 3D (ellipsoid-in-an-ellipsoid)
+* [Example 5](https://rangamanilabucsd.github.io/smart/examples/example5/example5.html): Simple cell signaling model in 3D (cube-in-a-cube)
+* [Example 6](https://rangamanilabucsd.github.io/smart/examples/example6/example6.html): Model of calcium dynamics in a neuron (sphere-in-a-sphere)
 
-## Functionality
+## Functionality documentation
 SMART is equipped to handle:
 * Reaction-diffusion with any number of species, reactions, and compartments.
-* Reaction-diffusion with boundary conditions between coupled sub-volumes and sub-surfaces (defined by marker values in the .xml file).
-* Reaction-diffusion in non-manifold meshes (experimental).
+* 3D-2D problems or 2D-1D problems; that is, you can solve a problem with many 3d sub-volumes coupled to many 2d sub-surfaces, or a problem with many 2d "sub-volumes" coupled to many 1d "sub-surfaces"
 * Conversion of units at run-time via [Pint](https://pint.readthedocs.io/en/stable/) so that models can be specified in whatever units are most natural/convenient to the user.
 * Specification of a time-dependent function either algebraically or from data (SMART will numerically integrate the data points at each time-step).
 * Customized reaction equations (e.g. irreversible Hill equation).
 
-SMART does not handle (it is possible to implement these features but would require a lot of work - contact author if interested):
-* Problems with coupled-physics spanning more than two dimensions. For example you may solve a problem with many 3d sub-volumes coupled to many 2d sub-surfaces, or a problem with many 2d "sub-volumes" coupled to many 1d "sub-surfaces" but a problem with 3d physics can't be coupled to a problem with 1d physics.
-* Sub-volumes embedded within sub-volumes (i.e. from any point inside the interior sub-volume, one must traverse two surfaces to get to the exterior of the full mesh)
-
-## Nomenclature
-Because SMART methods are viable in both 3 dimensional and 2 dimensional geometries we use the following nomenclature to define various functions in the code.
-
-Cell            : The element of the highest geometric dimension (e.g. "cell" refers to a tetrahedra in 3d, but a triangle in 2d).
-Facet           : The element of dimenion n-1 if n is the highest geometric dimension.
-Volume mesh     : A set of elements of the highest geometric dimension.
-Surface mesh    : A set of elements of dimension n-1 if n is the highest geometric dimension.
+The general form of the mixed-dimensional partial differential equations (PDEs) solved by SMART, along with mathematical details of the numerical implementation, are documented [here](https://rangamanilabucsd.github.io/smart/docs/math.html).
 
-"Cell" and "Volume" are used interchangeably (e.g. a volume mesh is a collection of cells). "Facet" and "Surface" are used interchangeably.
+Our API documentation can be accessed [here](https://rangamanilabucsd.github.io/smart/docs/api.html).
 
-## License
-STUBS is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-STUBS is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-GNU Lesser General Public License for more details.
+## Automated tests
+Upon pushing new code to the SMART repository, a number of tests run:
+* pre-commit tests
+* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects
+* Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
+* Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
+
+## Contributing guidelines
+
+Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
 
-You should have received a copy of the GNU Lesser General Public License
-along with STUBS. If not, see <http://www.gnu.org/licenses/>.
+### Dependencies
+* SMART uses [FEniCS](https://fenicsproject.org/) to assemble finite element matrices from the variational form
+* SMART uses [PETSc4py] to solve the resultant linear algebra systems.
+* SMART uses [pandas](https://pandas.pydata.org/) as an intermediate data structure to help organize and process models.
+* SMART uses [Pint](https://pint.readthedocs.io/en/stable/) for unit tracking and conversions.
+* SMART uses [matplotlib](https://matplotlib.org/) to generate plots in examples
+* SMART uses [sympy](https://www.sympy.org/) to allow users to input custom reactions and also to determine the appopriate solution techniques (e.g. testing for non-linearities).
+* SMART uses [numpy](https://numpy.org/) and [scipy](https://www.scipy.org/) for general array manipulations and basic calculations.
+* SMART uses [tabulate](https://pypi.org/project/tabulate/) to make ASCII tables.
+* SMART uses [termcolor](https://pypi.org/project/termcolor/) for colored terminal output.
 
-## Acknowledgements
+## License
+LGPL-3.0
 
-Thanks to [Christopher Lee](https://github.com/ctlee), [Yuan Gao](https://github.com/Rabona17), and [William Xu](https://github.com/willxu1234) for their valuable input and contributions to STUBS.
+## SMART development team
+* [Justin Laughlin](https://github.com/justinlaughlin) - original author of the repository
+* [Christopher Lee](https://github.com/ctlee)
+* [Emmet Francis](https://github.com/emmetfrancis)
+* [Jorgen Dokken](https://github.com/jorgensd)
+* [Henrik Finsberg](https://github.com/finsberg)
+
+Previous contributors:
+* [Yuan Gao](https://github.com/Rabona17)
+* [William Xu](https://github.com/willxu1234)
```

### Comparing `fenics-smart-2.0.1/fenics_smart.egg-info/PKG-INFO` & `fenics-smart-2.1.0/fenics_smart.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.0.1
+Version: 2.1.0
 Summary: SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -62,87 +62,109 @@
         
 Project-URL: homepage, https://rangamanilabucsd.github.io/smart
 Project-URL: repository, https://github.com/RangamaniLabUCSD/smart
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: examples
 Provides-Extra: all
 License-File: LICENSE
 
-Spatial Modelling Algorithms for Reaction-Transport [systems|models|equations]
-==============================
-[//]: # (Badges)
+[![Test fenics_smart](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml)
 [![PyPI](https://img.shields.io/pypi/v/fenics-smart)](https://pypi.org/project/fenics-smart/)
-
-
-SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models.
-SMART is highly suited for building systems biology models and simulating them as deterministic partial differential equations `[PDEs]` in realistic geometries using the Finite Element Method `[FEM]` - the integration of additional physics such as electro-diffusion or stochasticity may come in future updates.
-Systems biology models are converted by SMART into the appropriate systems of reaction-diffusion PDEs with proper boundary conditions.
-[FEniCS](https://fenicsproject.org/) is a core dependency of SMART which handles the assembly of finite element matrices as well as solving the resultant linear algebra systems.
+[![Deploy static content to Pages](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml)
+[![pre-commit](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml)
+# Spatial Modeling Algorithms for Reaction-Transport [systems|models|equations]
+
+## Statement of Need
+
+*Spatial Modeling Algorithms for Reactions and Transport* (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation for spatially-varying reaction-transport processes.
+SMART is based on the [FEniCS finite element library](https://fenicsproject.org/), provides a symbolic representation
+framework for specifying reaction pathways, and supports large and irregular cell geometries in 2D and 3D.
 
 - Documentation: https://rangamanilabucsd.github.io/smart
 - Source code: https://github.com/RangamaniLabUCSD/smart
 
 
 ## Installation
 
-### !!! IMPORTANT !!!
-Although FEniCS is a core dependency, because it has many different versions (2019.1, development, FEniCSx, etc.), is quite large, and is complicated to build, it is not packaged with SMART by default. The recommended way to use SMART is to create a container from one of the official FEniCS docker images and to pip install SMART from within the container.
+### Using docker (recommended)
+The simplest way to use `fenics-smart` is to use the provided docker image. You can get this image by pulling it from the github registry
+```
+docker pull ghcr.io/rangamanilabucsd/smart:latest
+```
+It is also possible to pull a specific version by changing the tag, e.g
+```
+docker pull ghcr.io/rangamanilabucsd/smart:v2.0.1
+```
+will use version 2.0.1.
 
-```bash
-# create a container using DOLFIN built on ubuntu 22.04 with Python 3.10
-jgl:~$ docker run -ti --init ghcr.io/scientificcomputing/fenics-gmsh:2023-04-21
-# pip install smart from within the container
-root@jgl:~$ python3 -m pip install fenics-smart
+In order to start a container you can use the [`docker run`](https://docs.docker.com/engine/reference/commandline/run/) command. For example the command
 ```
+docker run --rm -v $(pwd):/home/shared -w /home/shared -ti ghcr.io/rangamanilabucsd/smart:latest
+```
+will run the latest version and share your current working directory with the container.
 
-### Dependencies
-* SMART uses [FEniCS](https://fenicsproject.org/) to assemble finite element matrices as well as solve the resultant linear algebra systems.
-* SMART uses [pandas](https://pandas.pydata.org/) as an intermediate data structure to help organize and process models.
-* SMART uses [Pint](https://pint.readthedocs.io/en/stable/) for unit tracking and conversions.
-* SMART uses [matplotlib](https://matplotlib.org/) to automatically generate plots of min/mean/max (integrated over space) concentrations over time, as well as plots showing solver convergence.
-* SMART uses [sympy](https://www.sympy.org/) to allow users to input custom reactions and also to determine the appopriate solution techniques (e.g. testing for non-linearities).
-* SMART uses [numpy](https://numpy.org/) and [scipy](https://www.scipy.org/) for general array manipulations and basic calculations.
-* SMART uses [tabulate](https://pypi.org/project/tabulate/) to make pretty ASCII tables.
-* SMART uses [termcolor](https://pypi.org/project/termcolor/) for pretty terminal output so that simulations are more satisfying to watch.
+### Using pip
+`fenics-smart` is also available on [pypi](https://pypi.org/project/fenics-smart/) and can be installed with
+```
+python3 -m pip install fenics-smart
+```
+However this requires FEniCS version 2019.2.0 or later to already be installed. Currently, FEniCS version 2019.2.0 needs to be built [from source](https://bitbucket.org/fenics-project/dolfin/src/master/) or use some of the [pre-built docker images](https://github.com/orgs/scientificcomputing/packages?repo_name=packages)
+
+## Example usage
+The SMART repository contains a number of examples in the `examples` directory which also run as continuous integration tests (see "Automated Tests" below):
+* [Example 1](https://rangamanilabucsd.github.io/smart/examples/example1/example1.html): Formation of Turing patterns in 2D reaction-diffusion (rectangular domain)
+* [Example 2](https://rangamanilabucsd.github.io/smart/examples/example2/example2.html): Simple cell signaling model in 2D (ellipse)
+* [Example 3](https://rangamanilabucsd.github.io/smart/examples/example3/example3.html): Model of protein phosphorylation and diffusion in 3D (sphere)
+* [Example 4](https://rangamanilabucsd.github.io/smart/examples/example4/example4.html): Model of second messenger reaction-diffusion in 3D (ellipsoid-in-an-ellipsoid)
+* [Example 5](https://rangamanilabucsd.github.io/smart/examples/example5/example5.html): Simple cell signaling model in 3D (cube-in-a-cube)
+* [Example 6](https://rangamanilabucsd.github.io/smart/examples/example6/example6.html): Model of calcium dynamics in a neuron (sphere-in-a-sphere)
 
-## Functionality
+## Functionality documentation
 SMART is equipped to handle:
 * Reaction-diffusion with any number of species, reactions, and compartments.
-* Reaction-diffusion with boundary conditions between coupled sub-volumes and sub-surfaces (defined by marker values in the .xml file).
-* Reaction-diffusion in non-manifold meshes (experimental).
+* 3D-2D problems or 2D-1D problems; that is, you can solve a problem with many 3d sub-volumes coupled to many 2d sub-surfaces, or a problem with many 2d "sub-volumes" coupled to many 1d "sub-surfaces"
 * Conversion of units at run-time via [Pint](https://pint.readthedocs.io/en/stable/) so that models can be specified in whatever units are most natural/convenient to the user.
 * Specification of a time-dependent function either algebraically or from data (SMART will numerically integrate the data points at each time-step).
 * Customized reaction equations (e.g. irreversible Hill equation).
 
-SMART does not handle (it is possible to implement these features but would require a lot of work - contact author if interested):
-* Problems with coupled-physics spanning more than two dimensions. For example you may solve a problem with many 3d sub-volumes coupled to many 2d sub-surfaces, or a problem with many 2d "sub-volumes" coupled to many 1d "sub-surfaces" but a problem with 3d physics can't be coupled to a problem with 1d physics.
-* Sub-volumes embedded within sub-volumes (i.e. from any point inside the interior sub-volume, one must traverse two surfaces to get to the exterior of the full mesh)
-
-## Nomenclature
-Because SMART methods are viable in both 3 dimensional and 2 dimensional geometries we use the following nomenclature to define various functions in the code.
-
-Cell            : The element of the highest geometric dimension (e.g. "cell" refers to a tetrahedra in 3d, but a triangle in 2d).
-Facet           : The element of dimenion n-1 if n is the highest geometric dimension.
-Volume mesh     : A set of elements of the highest geometric dimension.
-Surface mesh    : A set of elements of dimension n-1 if n is the highest geometric dimension.
+The general form of the mixed-dimensional partial differential equations (PDEs) solved by SMART, along with mathematical details of the numerical implementation, are documented [here](https://rangamanilabucsd.github.io/smart/docs/math.html).
 
-"Cell" and "Volume" are used interchangeably (e.g. a volume mesh is a collection of cells). "Facet" and "Surface" are used interchangeably.
+Our API documentation can be accessed [here](https://rangamanilabucsd.github.io/smart/docs/api.html).
 
-## License
-STUBS is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-STUBS is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-GNU Lesser General Public License for more details.
+## Automated tests
+Upon pushing new code to the SMART repository, a number of tests run:
+* pre-commit tests
+* unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects
+* Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
+* Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
+
+## Contributing guidelines
+
+Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
 
-You should have received a copy of the GNU Lesser General Public License
-along with STUBS. If not, see <http://www.gnu.org/licenses/>.
+### Dependencies
+* SMART uses [FEniCS](https://fenicsproject.org/) to assemble finite element matrices from the variational form
+* SMART uses [PETSc4py] to solve the resultant linear algebra systems.
+* SMART uses [pandas](https://pandas.pydata.org/) as an intermediate data structure to help organize and process models.
+* SMART uses [Pint](https://pint.readthedocs.io/en/stable/) for unit tracking and conversions.
+* SMART uses [matplotlib](https://matplotlib.org/) to generate plots in examples
+* SMART uses [sympy](https://www.sympy.org/) to allow users to input custom reactions and also to determine the appopriate solution techniques (e.g. testing for non-linearities).
+* SMART uses [numpy](https://numpy.org/) and [scipy](https://www.scipy.org/) for general array manipulations and basic calculations.
+* SMART uses [tabulate](https://pypi.org/project/tabulate/) to make ASCII tables.
+* SMART uses [termcolor](https://pypi.org/project/termcolor/) for colored terminal output.
 
-## Acknowledgements
+## License
+LGPL-3.0
 
-Thanks to [Christopher Lee](https://github.com/ctlee), [Yuan Gao](https://github.com/Rabona17), and [William Xu](https://github.com/willxu1234) for their valuable input and contributions to STUBS.
+## SMART development team
+* [Justin Laughlin](https://github.com/justinlaughlin) - original author of the repository
+* [Christopher Lee](https://github.com/ctlee)
+* [Emmet Francis](https://github.com/emmetfrancis)
+* [Jorgen Dokken](https://github.com/jorgensd)
+* [Henrik Finsberg](https://github.com/finsberg)
+
+Previous contributors:
+* [Yuan Gao](https://github.com/Rabona17)
+* [William Xu](https://github.com/willxu1234)
```

### Comparing `fenics-smart-2.0.1/pyproject.toml` & `fenics-smart-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-smart"
-version = "2.0.1"
+version = "2.1.0"
 description = "SMART is a biophysical simulation library that provides a level of abstraction to models, making it easier for users to develop, share, and simulate their mathematical models"
 authors = [{name = "Justin Laughlin", email = "justinglaughlin@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "matplotlib",
     "numpy>=1.16.0",
     "pandas",
     "Pint",
     "scipy>=1.1.0",
     "sympy",
     "dataclasses",
     "cached-property",
     "tabulate",
     "termcolor",
     "termplotlib",
-    "meshio",
-    "gmsh"
 ]
 
 
 [project.urls]
 homepage = "https://rangamanilabucsd.github.io/smart"
 repository = "https://github.com/RangamaniLabUCSD/smart"
 
@@ -39,15 +36,23 @@
     "pytest",
     "pytest-cov",
 ]
 docs = [
    "jupyter-book",
    "sphinx-autoapi"
 ]
+examples = [
+    "meshio",
+    "gmsh",
+    "pyvista==0.38.4",
+    "panel",
+    "matplotlib"
+]
 all = [
+   "smart[examples]",
    "smart[test]",
    "smart[docs]",
    "smart[dev]"
 ]
 
 
 [tool.pytest.ini_options]
```

### Comparing `fenics-smart-2.0.1/smart/config.py` & `fenics-smart-2.1.0/smart/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Configuration settings for simulation: plotting, reaction types, solution output, etc.
+Configuration settings for simulation: logger formatting, solver configuration, other flags
 """
 import logging
 from logging import config as logging_config
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Any, Dict, Optional, Tuple, NamedTuple
 
@@ -23,15 +23,16 @@
 
 
 comm = d.MPI.comm_world
 rank = comm.rank
 size = comm.size
 root = 0
 fancy_format = (
-    "%(asctime)s %(rank)s%(name)s - %(levelname)s - %(message)s (%(filename)s:%(lineno)d)"
+    "%(asctime)s %(rank)s%(name)s - %(levelname)s - "
+    "%(newline)s%(message)s%(newline)s (%(filename)s:%(lineno)d)"
 )
 base_format = "%(asctime)s %(name)s - %(levelname)s - %(message)s (%(filename)s:%(lineno)d)"
 root_format = "ROOT -" + base_format
 
 
 class FormatType(str, Enum):
     default = "default"
@@ -44,23 +45,25 @@
     log_important = "log_important"
     log_urgent = "log_urgent"
     warning = "warning"
     timestep = "timestep"
     solverstep = "solverstep"
     assembly = "assembly"
     assembly_sub = "assembly_sub"
+    table = "table"
 
 
 class FormatOption(NamedTuple):
     buffer_color: str = "cyan"
     text_color: str = "white"
     filler_char: str = ""
     num_banners: int = 0
     new_lines: Tuple[int, int] = (0, 0)
     left_justify: bool = False
+    is_table: bool = False
 
 
 def format_type_to_options(format_type: FormatType) -> FormatOption:
     """Take a format type and return the corresponding options
 
     Parameters
     ----------
@@ -75,24 +78,26 @@
     Raises
     ------
     ValueError
         If provided format type does not exist.
     """
     if FormatType[format_type] == FormatType.default:
         return FormatOption()
+    if FormatType[format_type] == FormatType.table:
+        return FormatOption(is_table=True)
     elif FormatType[format_type] == FormatType.title:
         return FormatOption(
             text_color="magenta",
             num_banners=1,
             new_lines=(1, 0),
         )
     elif FormatType[format_type] == FormatType.subtitle:
         return FormatOption(
             text_color="green",
-            filler_char=".",
+            filler_char="",
             left_justify=True,
         )
     elif FormatType[format_type] == FormatType.data:
         return FormatOption(
             buffer_color="white",
             text_color="white",
             filler_char="",
@@ -119,49 +124,49 @@
             filler_char="",
             left_justify=True,
         )
     elif FormatType[format_type] == FormatType.log_important:
         return FormatOption(
             buffer_color="white",
             text_color="magenta",
-            filler_char=".",
+            filler_char="",
         )
     elif FormatType[format_type] == FormatType.log_urgent:
         return FormatOption(
             buffer_color="white",
             text_color="red",
-            filler_char=".",
+            filler_char="",
         )
     elif FormatType[format_type] == FormatType.warning:
         return FormatOption(
             buffer_color="magenta",
             text_color="red",
-            filler_char="!",
+            filler_char="",
             num_banners=2,
             new_lines=(1, 1),
         )
     elif FormatType[format_type] == FormatType.timestep:
         return FormatOption(
             text_color="red",
             num_banners=2,
-            filler_char=".",
+            filler_char="",
             new_lines=(1, 1),
         )
     elif FormatType[format_type] == FormatType.solverstep:
         return FormatOption(
             text_color="red",
             num_banners=1,
-            filler_char=".",
+            filler_char="",
             new_lines=(1, 1),
         )
     elif FormatType[format_type] == FormatType.assembly:
         return FormatOption(
             text_color="magenta",
             num_banners=0,
-            filler_char=".",
+            filler_char="",
             new_lines=(1, 0),
         )
     elif FormatType[format_type] == FormatType.assembly_sub:
         return FormatOption(
             text_color="magenta",
             num_banners=0,
             filler_char="",
@@ -212,22 +217,24 @@
     banner = colored(
         format_option.filler_char * (title_str_len + parity), format_option.buffer_color
     )
     return banner, title_str
 
 
 class FancyFormatter(logging.Formatter):
+    "Custom Formatter for logging"
+
     def format(self, record: logging.LogRecord) -> str:
         # Set the rank attribute with is a parameter in the `fancy_format``
         record.rank = f"CPU {rank}: " if size > 1 else ""
 
         # Extract the format options. Here we expect that `format_type` is provided
         # as part of the `extra` dictionary passed to the logger
         format_option = format_type_to_options(getattr(record, "format_type", FormatType.default))
-
+        record.newline = "\n" if format_option.is_table else ""
         # Create the formatter
         formatter = logging.Formatter(fancy_format)
         # Format the record
         out = formatter.format(record)
         # Now create banners and formatted text
         banner, formatted_out = format_message(out, format_option=format_option)
 
@@ -325,65 +332,63 @@
 
 
 @dataclass
 class SolverConfig(BaseConfig):
     """
     Parameters for solver.
 
-    :param final_t: End time of simulation
-    :param use_snes: Use PETScSNES solver if true, else use DOLFINs NewtonSolver
-    :param snes_preassemble_linear_system: If True separate linear components during assembly
-    :param initial_dt: Initial time-stepping
-    :param adjust_dt: A tuple (t, dt) of floats indicating when to next adjust the
-        time-stepping and to what value
-    :param dt: Number of digits for rounding `dt`
-    :param print_assembly: Print information during assembly process
-    :param dt_decrease_factor:
-    :param dt_increase_factor:
-    :param attempt_timestep_restart_on_divergence: Restart snes solver if it diverges
+    Args:
+        final_t: End time of simulation
+        use_snes: Use PETScSNES solver if true, else use DOLFINs NewtonSolver
+        snes_preassemble_linear_system: If True separate linear components during assembly
+        initial_dt: Initial time-stepping
+        adjust_dt: A tuple (t, dt) of floats indicating when to next adjust the
+            time-stepping and to what value
+        dt: Number of digits for rounding `dt`
+        print_assembly: Print information during assembly process
+        dt_decrease_factor:
+        dt_increase_factor:
+        attempt_timestep_restart_on_divergence: Restart snes solver if it diverges
+        reset_timestep_for_negative_solution: Reduce solver timestep is solution is negative
     """
 
     final_t: Optional[float] = None
     use_snes: bool = True
     snes_preassemble_linear_system: bool = False  #: .. warning:: FIXME Currently untested
     initial_dt: Optional[float] = None
     adjust_dt: Optional[Tuple[float, float]] = None
     time_precision: int = 6
     print_assembly: bool = True
-    dt_decrease_factor: float = 1.0  #: .. warning:: FIXME Currently unused parameter
-    dt_increase_factor: float = 1.0  #: .. warning:: FIXME Currently unused parameter
-    attempt_timestep_restart_on_divergence: bool = False  # testing in progress
+    attempt_timestep_restart_on_divergence: bool = False
     reset_timestep_for_negative_solution: bool = False
 
 
 @dataclass
 class FlagsConfig(BaseConfig):
     """
     Various flags
 
-    :param store_solutions: Store solutions to file.
-    :param allow_unused_components: Allow parameters not defined in any reaction to be
-        defined in any model.
-    :param print_verbose_info: Print detailed information about a model
+    Args:
+        allow_unused_components: Allow parameters not defined in any reaction to be
+            defined in any model.
+        print_verbose_info: Print detailed information about a model
     """
 
-    store_solutions: bool = True
     allow_unused_components: bool = False
     print_verbose_info: bool = True
 
 
 @dataclass
 class Config:
     """
     Configuration settings.
 
-    :param solver: Options for the solvers
-    :param flags: Various options
-    :param directory: Outputting options
-    :param loglevel: Logging options for FEniCS modules
+    Args:
+        solver: Options for the solvers
+        flags: Various options
     """
 
     solver: SolverConfig = field(default_factory=SolverConfig)
     flags: FlagsConfig = field(default_factory=FlagsConfig)
 
     @property
     def reaction_database(self) -> Dict[str, str]:
```

### Comparing `fenics-smart-2.0.1/smart/deprecation.py` & `fenics-smart-2.1.0/smart/deprecation.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.0.1/smart/mesh.py` & `fenics-smart-2.1.0/smart/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Wrapper around dolfin mesh class (originally for submesh implementation - possibly unneeded now)
+Wrapper around dolfin mesh class to define parent and child meshes for SMART simulations.
 """
 from typing import Dict, FrozenSet
 import logging
 
 import dolfin as d
 import numpy as np
 from cached_property import cached_property
@@ -135,89 +135,105 @@
                 "dx", domain=mesh, subdomain_data=self.mf["cells_uncombined"]
             )
 
 
 class ParentMesh(_Mesh):
     """
     Mesh loaded in from data. Submeshes are extracted from the ParentMesh based
-    on marker values from the .xml file.
+    on marker values from the .hdf5 or .xml file.
 
     Args:
-        mesh_filename (str): Name of mesh file
-        mesh_filetype (str): Extension of mesh, either 'xml' or 'hdf5'
-        name (str): Name of mesh
-        use_partition (bool): If `hdf5` mesh file is loaded,
+    * mesh_filename (str): Name of mesh file
+    * mesh_filetype (str): Extension of mesh, either 'xml' or 'hdf5'
+    * parent_mesh (str): Name of mesh
+    * use_partition (bool): If `hdf5` mesh file is loaded,
             choose if mesh should be read in with its current partition
     """
 
     mesh_filename: str
     mesh_filetype: str
     child_meshes: Dict[str, "ChildMesh"]
     parent_mesh: "ParentMesh"
     use_partition: bool
 
-    def __init__(self, mesh_filename: str, mesh_filetype, name, use_partition=False):
+    def __init__(
+        self,
+        mesh_filename: str,
+        mesh_filetype,
+        name,
+        use_partition=False,
+        mpi_comm=d.MPI.comm_world,
+    ):
         super().__init__(name)
         self.use_partition = use_partition
+        self.mpi_comm = mpi_comm
         if mesh_filetype == "xml":
             self.load_mesh_from_xml(mesh_filename)
         elif mesh_filetype == "hdf5":
             self.load_mesh_from_hdf5(mesh_filename, use_partition)
         self.mesh_filename = mesh_filename
         self.mesh_filetype = mesh_filetype
 
         self.child_meshes = dict()
         self.parent_mesh = self
 
     def get_mesh_from_id(self, id):
+        "Find the mesh that has the matching id."
         # find the mesh in that has the matching id
         for mesh in self.all_meshes.values():
             if mesh.id == id:
                 return mesh
 
     @property
     def all_meshes(self):
         return dict(list(self.child_meshes.items()) + list({self.name: self}.items()))
 
     def load_mesh_from_xml(self, mesh_filename):
+        "Load parent mesh from xml file `mesh_filename`"
         self.dolfin_mesh = d.Mesh(mesh_filename)
 
         self.dimensionality = self.dolfin_mesh.topology().dim()
         self.dolfin_mesh.init(self.dimensionality - 1)
         self.dolfin_mesh.init(self.dimensionality - 1, self.dimensionality)
         self.dolfin_mesh.init(self.dimensionality - 1, self.dimensionality)
 
         logger.info(f'XML mesh, "{self.name}", successfully loaded from file: {mesh_filename}!')
 
-    def load_mesh_from_hdf5(self, mesh_filename, use_partition=False, comm=d.MPI.comm_world):
+    def load_mesh_from_hdf5(self, mesh_filename, use_partition=False):
+        """
+        Load parent mesh from hdf5 file `mesh_filename`
+        Parallelize mesh if `use_partition` is True
+        """
+        comm = self.mpi_comm
         # mesh, mfs = common.read_hdf5(hdf5_filename)
         self.dolfin_mesh = d.Mesh(comm)
         hdf5 = d.HDF5File(self.dolfin_mesh.mpi_comm(), mesh_filename, "r")
         hdf5.read(self.dolfin_mesh, "/mesh", use_partition)
 
-        d.MPI.comm_world.Barrier()
+        if comm.size > 1:
+            d.MPI.comm_world.Barrier()
         hdf5.close()
 
         self.dimensionality = self.dolfin_mesh.topology().dim()
         self.dolfin_mesh.init(self.dimensionality - 1)
         self.dolfin_mesh.init(self.dimensionality - 1, self.dimensionality)
-        self.dolfin_mesh.init(self.dimensionality - 1, self.dimensionality)
 
         logger.info(f'HDF5 mesh, "{self.name}", successfully loaded from file: {mesh_filename}!')
 
     def _read_parent_mesh_function_from_file(self, dim):
         if self.mesh_filetype == "xml":
             mf = d.MeshFunction("size_t", self.dolfin_mesh, dim, value=self.dolfin_mesh.domains())
         elif self.mesh_filetype == "hdf5":
             mf = d.MeshFunction("size_t", self.dolfin_mesh, dim, value=0)
             # with d.HDF5File(self.dolfin_mesh.mpi_comm(), self.mesh_filename, 'r') as hdf5:
             # hdf5.read(mf, f'/mesh/{dim}')
             hdf5 = d.HDF5File(self.dolfin_mesh.mpi_comm(), self.mesh_filename, "r")
             hdf5.read(mf, f"/mf{dim}")
-            d.MPI.comm_world.Barrier()
+            if self.dolfin_mesh.mpi_comm().size > 1:
+                d.MPI.comm_world.Barrier()
             hdf5.close()
         return mf
 
     def read_parent_mesh_functions_from_file(self):
         """
         Read mesh function for parent mesh into :attr:`ParentMesh.mf`.
         """
@@ -280,19 +296,19 @@
     @property
     def child_volume_meshes(self):
         return [cm for cm in self.child_meshes.values() if cm.is_volume]
 
 
 class ChildMesh(_Mesh):
     """
-    Sub mesh of a parent mesh.
+    Sub-mesh of a parent mesh, defined by mesh markers.
 
     Params:
-        parent_mesh: The mesh owning the entities in the compartment
-        compartment: The compartment
+    * parent_mesh: The mesh owning the entities in the compartment
+    * compartment: The compartment object
     """
 
     intersection_map: Dict[FrozenSet[int], d.MeshFunction]
     intersection_map_parent: Dict[FrozenSet[int], d.MeshFunction]
     intersection_submesh: Dict[FrozenSet[int], d.Mesh]
     intersection_dx: Dict[FrozenSet[int], d.Measure]
     has_intersection: Dict[FrozenSet[int], bool]
@@ -430,15 +446,7 @@
         # add self to parent mesh's list of children meshes
         if self.parent_mesh:
             self.parent_mesh.child_meshes.update({self.name: self})
 
     def extract_submesh(self):
         mf_type = "cells" if self.is_volume else "facets"
         self.dolfin_mesh = d.MeshView.create(self.parent_mesh.mf[mf_type], self.primary_marker)
-
-    def init_marker_list_mesh_function(self):
-        "Child mesh functions require transfering data from parent mesh functions"
-        assert hasattr(self.parent_mesh, "mf")
-        assert self.marker_list is not None
-
-        # initialize
-        raise NotImplementedError("Need to check this")
```

### Comparing `fenics-smart-2.0.1/smart/model.py` & `fenics-smart-2.1.0/smart/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+"""Functions associated with the SMART model class
 """
-Model class. Consists of parameters, species, etc. and is used for simulation
-"""
+import pickle
 from collections import OrderedDict as odict
 from dataclasses import dataclass
 from decimal import Decimal
 from itertools import chain
 import logging
 
 import dolfin as d
@@ -31,39 +31,58 @@
     Parameter,
     ParameterContainer,
     Reaction,
     ReactionContainer,
     Species,
     SpeciesContainer,
     empty_sbmodel,
+    ParameterType,
 )
 from .solvers import smartSNESProblem
 from .units import unit
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Model:
-    """
-    Main smart class. Consists of parameters,
-    species, compartments, reactions, and can be simulated.
+    """SMART model class: consists of parameters,
+    species, compartments, reactions.
+
+    Args:
+        pc: Parameter container, initialized in model_assembly
+        sc: Species container, initialized in model_assembly
+        cc: Compartment container, initialized in model_assembly
+        rc: Reaction container, initialized in model_assembly
+        config: configuration object initialized in config.py
+        parent_mesh: ParentMesh object initialized in mesh.py
+        name (optional): string specifying a name for your model
+
+    .. note::
+        Given a parent mesh
+        and solver, the system can be solved for spatiotemporal dynamics.
+        Object is initialized by calling:
+
+        .. code:: python
+
+            model = model.Model(pc, sc, cc, rc, config, parent_mesh)
     """
 
     pc: ParameterContainer
     sc: SpeciesContainer
     cc: CompartmentContainer
     rc: ReactionContainer
     config: Config
     # solver_system: smart.solvers.SolverSystem
     parent_mesh: ParentMesh
     name: str = ""
 
     def to_dict(self):
+        """Convert model information to Dict"""
         parameters = self.pc.to_dicts()
         species = self.sc.to_dicts()
         compartments = self.cc.to_dicts()
         reactions = self.rc.to_dicts()
         return {
             "name": self.name,
             "parameters": parameters,
@@ -73,27 +92,41 @@
             "parent_mesh_filename": self.parent_mesh.mesh_filename,
             "parent_mesh_filetype": self.parent_mesh.mesh_filetype,
             "config": self.config.__dict__,
         }
 
     @classmethod
     def from_dict(cls, input_dict):
+        """Read model information from Dict"""
         pc, sc, cc, rc = empty_sbmodel()
         pc.add([Parameter.from_dict(parameter) for parameter in input_dict["parameters"]])
         sc.add([Species.from_dict(species) for species in input_dict["species"]])
         cc.add([Compartment.from_dict(compartment) for compartment in input_dict["compartments"]])
         rc.add([Reaction.from_dict(reaction) for reaction in input_dict["reactions"]])
         config = Config()
         config.__dict__ = input_dict["config"]
         parent_mesh = ParentMesh(
             input_dict["parent_mesh_filename"], input_dict["parent_mesh_filetype"]
         )
         return cls(pc, sc, cc, rc, config, parent_mesh, input_dict["name"])
 
+    def to_pickle(self, filename):
+        """Save model information to file by pickling"""
+        with open(filename, "wb") as f:
+            pickle.dump(self.to_dict(), f)
+
+    @classmethod
+    def from_pickle(cls, filename):
+        """Read model information from file by unpickling"""
+        with open(filename, "rb") as f:
+            input_dict = pickle.load(f)
+        return cls.from_dict(input_dict)
+
     def __post_init__(self):
+        """Initialize solver-related parameters, timers, and MPI."""
         # # Check that solver_system is valid
 
         # FunctionSpaces, Functions, etc
         self.V = dict()
         self.u = dict()
 
         self.fc = FluxContainer()
@@ -130,57 +163,54 @@
             stopwatch_name: Stopwatch(stopwatch_name, print_buffer=print_buffer)
             for stopwatch_name in stopwatch_names
         }
 
         # Functional forms
         self.forms = FormContainer()
 
-        # MPI
-        self.mpi_comm_world = d.MPI.comm_world
+        # MPI - define to be consistent with mesh
+        self.mpi_comm_world = self.parent_mesh.mpi_comm
         self.mpi_rank = self.mpi_comm_world.rank
         self.mpi_size = self.mpi_comm_world.size
         self.mpi_root = 0
 
         if self.mpi_size > 1:
             logger.info(
                 f"CPU {self.mpi_rank}: Model '{self.name}' "
                 f"has been parallelized (size={self.mpi_size}).",
                 extra=dict(format_type="log_urgent"),
             )
 
     @property
     def mpi_am_i_root(self):
+        """Returns True if current process is root"""
         return self.mpi_rank == self.mpi_root
 
     @property
     def child_meshes(self):
+        """Returns all child meshes in current parent mesh"""
         return self.parent_mesh.child_meshes
 
     @cached_property
     def min_dim(self):
+        """Returns minimum dimension in current model"""
         dim = min([comp.dimensionality for comp in self.cc])
         self.parent_mesh.min_dim = dim
         return dim
 
     @cached_property
     def max_dim(self):
+        """Returns maximum dimension in current model"""
         dim = max([comp.dimensionality for comp in self.cc])
         self.max_dim = dim
         self.parent_mesh.max_dim = dim
         return dim
 
-    # ===========================================
-    # Model - Initialization
-    # ===========================================
     def initialize(self, initialize_solver=True):
-        """
-        Notes:
-        * Now works with sub-volumes
-        * Removed scale_factor (too ambiguous)
-        """
+        """Main model initialization function, split into 5 subfunctions"""
 
         # Solver related parameters
         self._base_t = Decimal("0." + (self.config.solver["time_precision"] - 1) * "0" + "1")
         self.t = self.rounded_decimal(0.0)
         self.dt = self.rounded_decimal(self.config.solver["initial_dt"])
         self.final_t = self.rounded_decimal(self.config.solver["final_t"])
         assert self.config.solver["time_precision"] in range(1, 30)
@@ -201,15 +231,15 @@
             self.pc.print()
             self.sc.print()
             self.cc.print()
             self.print_meshes()
             self.rc.print()
 
     def _init_1(self):
-        "Checking validity of model"
+        """Checking validity of model"""
         logger.debug("Checking validity of model (step 1 of ZZ)", extra=dict(format_type="title"))
         self._init_1_1_check_mesh_dimensionality()
         self._init_1_2_check_namespace_conflicts()
         self._init_1_3_check_parameter_dimensionality()
         logger.debug(
             "Step 1 of initialization completed successfully!",
             extra=dict(text_color="magenta"),
@@ -233,15 +263,15 @@
         self._init_2_7_get_species_compartment_indices()
         logger.debug(
             "Step 2 of initialization completed " "successfully!",
             extra=dict(text_color="magenta"),
         )
 
     def _init_3(self):
-        "Mesh-related initializations"
+        """Mesh-related initializations"""
         logger.debug(
             "Mesh-related Initializations (step 3 of ZZ)",
             extra=dict(format_type="title"),
         )
         self._init_3_1_define_child_meshes()
         self._init_3_2_read_parent_mesh_functions_from_file()
         self._init_3_3_extract_submeshes()
@@ -252,40 +282,49 @@
         self._init_3_7_get_integration_measures()
         logger.debug(
             "Step 3 of initialization completed successfully!",
             extra=dict(format_type="log_important"),
         )
 
     def _init_4(self):
-        "Dolfin function initializations"
+        """Dolfin function initializations"""
         logger.debug("Dolfin Initializations (step 4 of ZZ)", extra=dict(format_type="title"))
         self._init_4_0_initialize_dolfin_parameters()
         self._init_4_1_get_active_compartments()
         self._init_4_2_define_dolfin_function_spaces()
         self._init_4_3_define_dolfin_functions()
         self._init_4_4_get_species_u_v_V_dofmaps()
         self._init_4_5_name_functions()
         self._init_4_6_check_dolfin_function_validity()
         self._init_4_7_set_initial_conditions()
 
     def _init_5(self, initialize_solver):
+        """Convert reactions to fluxes and define variational form.
+        If initialize_solver is true, also initialize solver.
+        """
         logger.debug(
             "Dolfin fluxes, forms, and problems+solvers (step 5 of ZZ)",
             extra=dict(
                 format_type="title",
             ),
         )
         self._init_5_1_reactions_to_fluxes()
         self._init_5_2_create_variational_forms()
         if initialize_solver:
             self.initialize_discrete_variational_problem_and_solver()
 
     # Step 1 - Checking model validity
 
     def _init_1_1_check_mesh_dimensionality(self):
+        """Dimensionality checks:
+
+        * Error if max_dim - min_dim is greater than 1
+        * Error if max_dim (from compartments) is greater than dimensionality of parent mesh
+        * Warning if max_dim is less than dimensionality of parent mesh
+        """
         logger.debug(
             "Check that mesh/compartment dimensionalities match",
             extra=dict(format_type="log"),
         )
 
         if (self.max_dim - self.min_dim) not in [0, 1]:
             raise ValueError(
@@ -307,14 +346,21 @@
                 extra=dict(format_type="warning"),
             )
 
         for compartment in self.cc:
             compartment.is_volume = compartment.dimensionality == self.max_dim
 
     def _init_1_2_check_namespace_conflicts(self):
+        """Namespace checks:
+
+        * no repeated names of parameters/species/compartments/reactions
+        * no use of x[0], x[1], x[2], t, or unit_scale_factor as names
+        * no two compartments share the same marker number
+        * no compartment has a marker value of 0
+        """
         logger.debug("Checking for namespace conflicts", extra=dict(format_type="log"))
         self._all_keys = set()
         containers = [self.pc, self.sc, self.cc, self.rc]
         for keys in [c.keys for c in containers]:
             self._all_keys = self._all_keys.union(keys)
         if sum([c.size for c in containers]) != len(self._all_keys):
             raise ValueError(
@@ -344,31 +390,30 @@
                     raise ValueError(f"Two compartments have the same marker: {marker}")
                 elif marker == 0:
                     raise ValueError("Marker cannot have the value 0")
                 else:
                     self._all_markers.add(marker)
 
     def _init_1_3_check_parameter_dimensionality(self):
+        """Check no objects reference a higher spatial dimension than max_dim"""
         if "x[2]" in self._all_keys and self.max_dim < 3:
             raise ValueError(
                 "An object has the variable name 'x[2]' but there "
                 "are less than 3 spatial dimensions."
             )
         if "x[1]" in self._all_keys and self.max_dim < 2:
             raise ValueError(
                 "An object has the variable name 'x[1]' but there are "
                 "less than 2 spatial dimensions."
             )
 
     # Step 2 - Cross-container Dependent Initialization
 
     def _init_2_1_reactions_to_symbolic_strings(self):
-        """
-        Turn all reactions into unsigned symbolic flux strings
-        """
+        """Turn all reactions into unsigned symbolic flux strings"""
         logger.debug(
             "Turning reactions into unsigned symbolic flux strings",
             extra=dict(format_type="log"),
         )
 
         for reaction in self.rc:
             # Mass action has a forward and reverse flux
@@ -404,14 +449,15 @@
 
             else:
                 raise ValueError(
                     "Reaction %s does not seem to have an associated equation" % reaction.name
                 )
 
     def _init_2_2_check_reaction_validity(self):
+        """Confirms that all reactions have parameters/species defined"""
         logger.debug(
             "Make sure all reactions have parameters/species defined",
             extra=dict(format_type="log"),
         )
         # Make sure all reactions have parameters/species defined
         for reaction in self.rc:
             for eqn_str in [reaction.eqn_f_str, reaction.eqn_r_str]:
@@ -425,14 +471,15 @@
                     diff_set = var_set.difference(param_set.union(species_set))
                     raise NameError(
                         f"Reaction {reaction.name} refers to a parameter or "
                         f"species ({diff_set}) that is not in the model."
                     )
 
     def _init_2_3_link_reaction_properties(self):
+        """Link parameters, species, and compartments to reactions"""
         logger.debug(
             "Linking parameters, species, and compartments to reactions",
             extra=dict(format_type="log"),
         )
 
         for reaction in self.rc:
             reaction.parameters = {
@@ -485,14 +532,18 @@
                     )
                 else:
                     reaction.topology = "volume_surface_volume"
             else:
                 raise ValueError("Number of compartments involved in a flux must be in [1,2,3]!")
 
     def _init_2_4_check_for_unused_parameters_species_compartments(self):
+        """
+        If :code:`self.config.flags["allow_unused_components"]` is true,
+        then unused objects are removed
+        """
         logger.debug(
             "Checking for unused parameters, species, or compartments",
             extra=dict(format_type="log"),
         )
 
         all_parameters = set(chain.from_iterable([r.parameters for r in self.rc]))
         all_species = set(chain.from_iterable([r.species for r in self.rc]))
@@ -540,74 +591,80 @@
                     "Removing unused compartment(s) from model!",
                     extra=dict(format_type="log_urgent"),
                 )
             else:
                 raise ValueError(print_str)
 
     def _init_2_5_link_compartments_to_species(self):
+        """Linking compartments and compartment dimensionality to species"""
         logger.debug(
             "Linking compartments and compartment dimensionality to species",
             extra=dict(format_type="log"),
         )
         for species in self.sc:
             species.compartment = self.cc[species.compartment_name]
             species.dimensionality = self.cc[species.compartment_name].dimensionality
 
     def _init_2_6_link_species_to_compartments(self):
+        """Links species to compartments - a species is considered to be
+        "in a compartment" if it is involved in a reaction there
+        """
         logger.debug("Linking species to compartments", extra=dict(format_type="log"))
         # An species is considered to be "in a compartment" if it is
         # involved in a reaction there
         for species in self.sc:
             species.compartment.species.update({species.name: species})
         for compartment in self.cc:
             compartment.num_species = len(compartment.species)
 
     def _init_2_7_get_species_compartment_indices(self):
+        """Store dof indices for species for each compartment"""
         logger.debug(
             "Getting indices for species for each compartment",
             extra=dict(format_type="log"),
         )
         for compartment in self.cc:
             index = 0
             for species in list(compartment.species.values()):
                 species.dof_index = index
                 index += 1
 
     # Step 3 - Mesh Initializations
     def _init_3_1_define_child_meshes(self):
+        """Initialize all ChildMesh objects"""
         logger.debug("Defining child meshes", extra=dict(format_type="log"))
         # Check that there is a parent mesh loaded
         if not isinstance(self.parent_mesh, ParentMesh):
             raise ValueError("There is no parent mesh.")
 
         # Define child meshes
         for comp in self.cc:
             comp.mesh = ChildMesh(self.parent_mesh, comp)
 
         # Check validity (one child mesh for each compartment)
         assert len(self.child_meshes) == self.cc.size
 
     def _init_3_2_read_parent_mesh_functions_from_file(self):
-        """
-        Reads mesh functions from an .xml or .hdf5 file.
+        """Reads mesh functions from an .xml or .hdf5 file.
         If told that a child mesh consists of a list of markers,
         creates a separate mesh function
         for the list and for the combined list (can be used for post-processing)
         """
         logger.debug("Defining parent mesh functions", extra=dict(format_type="log"))
         self.parent_mesh.read_parent_mesh_functions_from_file()
 
     def _init_3_3_extract_submeshes(self):
-        """Use dolfin.MeshView.create() to extract submeshes"""
+        """Use :code:`dolfin.MeshView.create()` to extract submeshes"""
         logger.debug("Extracting submeshes using MeshView", extra=dict(format_type="log"))
         # Loop through child meshes and extract submeshes
         for child_mesh in self.child_meshes.values():
             child_mesh.extract_submesh()
 
     def _init_3_4_build_submesh_mappings(self):
+        """Build MeshView mappings between all child mesh pairs"""
         logger.debug(
             "Building MeshView mappings between all child mesh pairs",
             extra=dict(format_type="log"),
         )
 
         # not creating maps with build_mapping() will lead to a
         # segfault when trying to assemble
@@ -629,61 +686,74 @@
                             ),
                             extra=dict(format_type="log"),
                         )
                         continue
                 child_mesh.dolfin_mesh.build_mapping(sibling_volume_mesh.dolfin_mesh)
 
     def _init_3_7_get_integration_measures(self):
+        """Get integration measures for parent mesh and child meshes"""
         logger.debug(
             "Getting integration measures for parent mesh and child meshes",
             extra=dict(format_type="log"),
         )
         for mesh in self.parent_mesh.all_meshes.values():
             mesh.get_integration_measures()
 
     def _init_4_0_initialize_dolfin_parameters(self):
-        """
-        Create dolfin objects for each parameter
-        Because we don't want to re-create dolfin constants
-        each time (will cause fenics to recompile form)
-        we only define them once here. That means that once
-        the model is initialized, changing a parameter's
+        """Create dolfin objects for each parameter.
+        If we were to re-create dolfin constants
+        each time, FEniCS will recompile the form
+        so we only define them once here.
+        Therefore, once the model is initialized, changing a parameter's
         value does not change the underlying dolfin object.
-        Values must be assigned via paramter.dolfin_constant.assign()
+        Values must be assigned via :code:`parameter.dolfin_constant.assign()`
         """
         # Create a dolfin.Constant() for constant parameters
         for parameter in self.pc.values:
-            if parameter.type == "constant":
+            if parameter.type == ParameterType.constant:
                 parameter.dolfin_constant = d.Constant(parameter.value)
-            elif parameter.type == "expression" and not parameter.use_preintegration:
+            elif parameter.type == ParameterType.expression and not parameter.use_preintegration:
                 parameter.dolfin_expression = d.Expression(
                     sym.printing.ccode(parameter.sym_expr), t=self.T, degree=1
                 )
-            elif parameter.type == "expression" and parameter.use_preintegration:
+            elif parameter.type == ParameterType.expression and parameter.use_preintegration:
                 parameter.dolfin_constant = d.Constant(parameter.value)
-            elif parameter.type == "from_file":
+            elif parameter.type == ParameterType.from_file:
                 parameter.dolfin_constant = d.Constant(parameter.value)
 
     def _init_4_1_get_active_compartments(self):
-        """
-        Arrange the compartments based on the number of degrees of freedom they have
+        """Arrange the compartments based on the number of degrees of freedom they have
         (We want to have the highest number of dofs first)
         """
         # addressing https://github.com/justinlaughlin/smart/issues/36
         self._active_compartments = list(self.cc.Dict.values())
         self._all_compartments = list(self.cc.Dict.values())
+        it_idx = 0
+        rm_idx = np.array([])
         for compartment in self._active_compartments:
             if compartment.num_species < 1:
-                self._active_compartments.remove(compartment)
+                rm_idx = np.append(rm_idx, it_idx)
+            it_idx = it_idx + 1
+        for i in range(len(rm_idx)):
+            rm_cur = int(rm_idx[i])
+            del self._active_compartments[rm_cur]
+            rm_idx = rm_idx - 1  # adjust indices to compensate after deleting
         for idx, compartment in enumerate(self._active_compartments):
             compartment.dof_index = idx
 
     # Step 4 - Dolfin Functions
 
     def _init_4_2_define_dolfin_function_spaces(self):
+        """Define dolfin function spaces for compartments
+        For each compartment, a P1 (linear shape functions for a tri or tet element)
+        vector function space is used, with the vector dimensionality given
+        by the number of species in the compartment.
+        The mixed function space W is the product space of all vector function
+        spaces of individual compartments
+        """
         logger.debug(
             "Defining dolfin function spaces for compartments",
             extra=dict(format_type="log"),
         )
         # Aliases
         max_compartment_name = max([len(compartment_name) for compartment_name in self.cc.keys])
 
@@ -711,54 +781,43 @@
                 )
 
         self.V = [compartment.V for compartment in self._active_compartments]
         # Make the MixedFunctionSpace
         self.W = d.MixedFunctionSpace(*self.V)
 
     def _init_4_3_define_dolfin_functions(self):
-        """
-        Some notes on functions in VectorFunctionSpaces:
-        u.sub(idx) gives us a shallow copy to the idx sub-function of u.
-        This is useful when we want to look at function values
-
-        u.split()[idx] is equivalent to u.sub(idx)
-
-        d.split(u)[idx] (same thing as ufl.split(u)) gives us
-        ufl objects (ufl.indexed.Indexed)
-        that can be used in variational formulations.
-
-        u.sub(idx) can be used in a variational formulation but
-        it won't behave properly.
-        E.g. consider u as a 2d function
-        V  = d.VectorFunctionSpace(mesh, "P", 1, dim=2)
-        u  = d.Function(V)
-        u0 = u.sub(0); u1 = u.sub(1)
-        v  = d.TestFunction(V)
-        v0 = v[0]; v1 = v[1]
-        F  = u0*v0*dx + u1*v1*dx
-        G  = d.inner(u,v)*dx
-        get_F    = lambda F: d.assemble(F).get_local()
-        get_dFdu = lambda F,u: d.assemble(d.derivative(F,u)).array()
-        (get_F(F) == get_F(G)).all() # True
-        (get_dFdu(F,u) == get_dFdu(G,u)).all() # False
-
-        Using u0,u1 = d.split(u) will give the right results
-
-        For TestFunctions/TrialFunctions, we will always get a
-        ufl.indexed.Indexed object
-        # type(v) == d.function.argument.Argument
-        v = d.TestFunction(V)
-        v[0] == d.split(v)[0]
-        # type(v_) == tuple(ufl.indexed.Indexed, ufl.indexed.Indexed)
-        v_ = d.TestFunctions(V)
-        v_[0] == v[0] == d.split(v)[0]
+        """Define test functions and trial functions in the mixed function space
 
-        For a MixedFunctionSpace e.g. W=d.MixedFunctionSpace(*[V1,V2])
-        we can use sub() to get the subfunctions
+        .. note::
+            Some notes on functions in VectorFunctionSpaces:
+            :code:`u.sub(idx)` gives us a shallow copy to the idx sub-function of
+            :code:`u`.
+            This is useful when we want to look at function values
+            :code:`u.split()[idx]` is equivalent to :code:`u.sub(idx)`
+
+            :code:`d.split(u)[idx]` (same thing as ufl.split(u)) gives us
+            ufl objects (:code:`ufl.indexed.Indexed`)
+            that can be used in variational formulations.
+
+            :code:`u.sub(idx)` can be used in a variational formulation but
+            it won't behave properly.
+
+            For TestFunctions/TrialFunctions, we will always get a
+            :code:`ufl.indexed.Indexed` object
+
+            .. code python
+                # type(v) == d.function.argument.Argument
+                v = d.TestFunction(V)
+                v[0] == d.split(v)[0]
+                # type(v_) == tuple(ufl.indexed.Indexed, ufl.indexed.Indexed)
+                v_ = d.TestFunctions(V)
+                v_[0] == v[0] == d.split(v)[0]
 
+            For a MixedFunctionSpace e.g. :code:`W=d.MixedFunctionSpace(*[V1,V2])`
+            we can use :code:`sub()` to get the subfunctions
         """
         logger.debug("Defining dolfin functions", extra=dict(format_type="log"))
         # dolfin functions created from MixedFunctionSpace
         self.u["u"] = d.Function(self.W)
         # self.u['k'] = d.Function(self.W)
         self.u["n"] = d.Function(self.W)
 
@@ -790,14 +849,15 @@
             compartment.ut = sub(self.ut, cidx)  # self.ut[cidx]
             compartment.v = sub(self.v, cidx)  # self.v[cidx]
 
         # save these in model
         self._usplit = [c._usplit["u"] for c in self._active_compartments]
 
     def _init_4_4_get_species_u_v_V_dofmaps(self):
+        """Extract subfunctions, function spaces, dofmap for each species"""
         logger.debug(
             "Extracting subfunctions/function spaces/dofmap for each species",
             extra=dict(format_type="log"),
         )
         for compartment in self._active_compartments:
             # loop through species and add the name/index
             for species in compartment.species.values():
@@ -809,27 +869,34 @@
                     # compartment.u[key].sub(species.dof_index)
                     species.u[key] = sub(compartment.u[key], species.dof_index)
                     # compartment.u[key].sub(species.dof_index)
                     species._usplit[key] = sub(compartment._usplit[key], species.dof_index)
                 species.ut = sub(compartment.ut, species.dof_index)
 
     def _init_4_5_name_functions(self):
+        """Assign function names based on compartment name, species index, and species name"""
         logger.debug("Naming functions and subfunctions", extra=dict(format_type="log"))
         for compartment in self._active_compartments:
             # name of the compartment function
             for key in self.u.keys():
                 compartment.u[key].rename(f"{compartment.name}_{key}", "")
                 # loop through species and add the name/index
                 for species in compartment.species.values():
                     sidx = species.dof_index
                     if compartment.num_species > 1:
                         species.u[key].rename(f"{compartment.name}_{sidx}_{species.name}_{key}", "")
 
     def _init_4_6_check_dolfin_function_validity(self):
-        "Sanity check... If an error occurs here it is likely an internal bug..."
+        """
+        Checks to confirm that dolfin functions were created correctly:
+
+        * function size in compartment == dof in that compartment
+        * number of sub-spaces in compartment == number of species in compartment
+        * function space of compartment matches sub-space of W
+        """
         logger.debug(
             "Checking that dolfin functions were created correctly",
             extra=dict(format_type="log"),
         )
         # sanity check
         for compartment in self._active_compartments:  # self.cc:
             idx = compartment.dof_index
@@ -850,39 +917,48 @@
                     assert compartment.u[ukey].num_sub_spaces() == compartment.num_species
 
             # function space matches W.sub(idx)
             for func in list(compartment.u.values()) + [compartment.v]:
                 assert func.function_space().id() == self.W.sub_space(idx).id()
 
     def _init_4_7_set_initial_conditions(self):
-        "Sets the function values to initial conditions"
+        """
+        Sets the function values to initial conditions,
+        either based on an expression given by a string
+        or a numerical value (float)
+        (see model.dolfin_set_function_values for further details)
+        """
         logger.debug("Set function values to initial conditions", extra=dict(format_type="log"))
         for species in self.sc:
             for ukey in species.u.keys():
                 if isinstance(species.initial_condition, float) or not isinstance(
                     species.initial_condition, str
                 ):
                     self.dolfin_set_function_values(species, ukey, species.initial_condition)
                 else:
                     self.dolfin_set_function_values(
                         species, ukey, species.initial_condition_expression
                     )
 
     def _init_5_1_reactions_to_fluxes(self):
+        """Convert reactions to flux objects"""
         logger.debug("Convert reactions to flux objects", extra=dict(format_type="log"))
         for reaction in self.rc:
             reaction.reaction_to_fluxes()
             self.fc.add(reaction.fluxes)
 
     def _init_5_2_create_variational_forms(self):
         """
         Setup the variational forms in dolfin
         Forms:
-        F(u;v) =    Muform      +   Munform   +       Dform         +         Rform           = 0
-                 linear wrt u         (v)         linear wrt u       possibly nonlinear wrt u
+
+        .. code:: python
+
+            F(u;v) =    Muform    + Munform   +    Dform     +     Rform              = 0
+                    linear wrt u      (v)      linear wrt u  possibly nonlinear wrt u
         """
         logger.debug("Creating functional forms", extra=dict(format_type="log"))
 
         # default dictionary (linear w.r.t all compartment functions)
         linear_wrt_comp = {k: True for k in self.cc.keys}
         # nonlinear_wrt_comp = {k: False for k in self.cc.keys}
 
@@ -970,15 +1046,15 @@
                     species,
                     "mass_un",
                     mass_form_units,
                     True,
                     linear_wrt_comp,
                 )
             )
-        # FIXME: `has_diffusive_forms` is only in commeted out code of
+        # FIXME: `has_diffusive_forms` is only in commented out code of
         # `initialize_discrete_variational_problem_and_solver`
         for compartment in self.cc:
             diffusive_forms = [
                 f
                 for f in self.forms
                 if f.compartment.name == compartment.name and f.form_type == "diffusion"
             ]
@@ -988,14 +1064,20 @@
                     extra=dict(format_type="log"),
                 )
                 compartment.has_diffusive_forms = False
             else:
                 compartment.has_diffusive_forms = True
 
     def initialize_discrete_variational_problem_and_solver(self):
+        """
+        Formulate problem for Newton iterations
+        and configure solver - currently, only using SNES in PETSc
+        is supported, the dolfin MixedNonlinearVariationalSolver
+        is not tested in this context
+        """
         logger.debug(
             "Formulating problem as F(u;v) == 0 for newton iterations",
             extra=dict(format_type="log"),
         )
         # self.all_forms = sum([f.form for f in self.forms])
         # self.problem = d.NonlinearVariationalProblem(self.all_forms, self.u['u'], bcs=None)
         # Aliases
@@ -1048,15 +1130,17 @@
             )
 
             self.problem.init_petsc_matnest()
             self.problem.init_petsc_vecnest()
             if len(self.problem.global_sizes) == 1:
                 self._ubackend = u[0].vector().vec().copy()
             else:
-                self._ubackend = PETSc.Vec().createNest([usub.vector().vec().copy() for usub in u])
+                self._ubackend = PETSc.Vec().createNest(
+                    [usub.vector().vec().copy() for usub in u], comm=self.mpi_comm_world
+                )
 
             self.solver = PETSc.SNES().create(self.mpi_comm_world)
 
             # Define the function/jacobian blocks
             self.solver.setFunction(self.problem.F, self.problem.Fpetsc_nest)
             self.solver.setJacobian(self.problem.J, self.problem.Jpetsc_nest)
             self.solver.setType("newtonls")
@@ -1067,43 +1151,47 @@
                 logger.debug("  " + str(it) + " SNES Function norm " + "{:e}".format(fgnorm))
 
             self.solver.setMonitor(monitor)
             opts = PETSc.Options()
             opts["snes_linesearch_type"] = "l2"
             self.solver.setFromOptions()
 
-            # These are some reasonable preconditioner/linear solver settings for block systems
-            # Krylov solver
-            # biconjugate gradient stabilized. in most cases probably the best option
-            self.solver.ksp.setType("bcgs")
-            self.solver.ksp.setTolerances(rtol=1e-5)
-            # Some other reasonable krylov solvers: (I don't think they work with block systems)
-            # bcgsl, ibcgs (improved stabilized bcgs)
-            # fbcgsr, fbcgs (flexible bcgs)
-
-            # Field split preconditioning
-            # Note from Emmet - can we solve this directly using LU? (suggestion from Marie)
-            # self.solver.ksp.pc.setType("lu")
-            self.solver.ksp.pc.setType("fieldsplit")
-            # Set the indices
-            nest_indices = self.problem.Jpetsc_nest.getNestISs()[0]
-            nest_indices_tuples = [(str(i), val) for i, val in enumerate(nest_indices)]
-            # self.solver.ksp.pc.setFieldSplitIS(("0", is_0), ("1", is_1))
-            self.solver.ksp.pc.setFieldSplitIS(*nest_indices_tuples)
-            # 0 == 'additive' [jacobi], 1 == gauss-seidel
-            self.solver.ksp.pc.setFieldSplitType(1)
-            subksps = self.solver.ksp.pc.getFieldSplitSubKSP()
-            for i, subksp in enumerate(subksps):
-                # subksp.setType('preonly')
-                # # If there is not diffusion then this is really just a distributed set of ODEs
-                # if not self._active_compartments[i].has_diffusive_forms:
-                #     subksp.pc.setType('none')
-                subksp.setType("preonly")
-                subksp.pc.setType("hypre")
-
+            # May look into using LU in all cases if possible (seems to converge very slowly)
+            if self.problem.is_single_domain:
+                # If only modeling species within a single domain
+                # (other domains may still contribute as BCs),
+                # then just use hypre (cannot use field split without multiple domains)
+                self.solver.ksp.setType("bcgs")
+                self.solver.ksp.setTolerances(rtol=1e-5)
+                self.solver.ksp.pc.setType("hypre")
+            else:  # Field split preconditioning:
+                # These are some reasonable preconditioner/linear solver settings for block systems
+                # Krylov solver
+                # biconjugate gradient stabilized. in most cases probably the best option
+                self.solver.ksp.setType("bcgs")
+                self.solver.ksp.setTolerances(rtol=1e-5)
+                # Some other reasonable krylov solvers: (don't think they work with block systems)
+                # bcgsl, ibcgs (improved stabilized bcgs)
+                # fbcgsr, fbcgs (flexible bcgs)
+                self.solver.ksp.pc.setType("fieldsplit")
+                # Set the indices
+                nest_indices = self.problem.Jpetsc_nest.getNestISs()[0]
+                nest_indices_tuples = [(str(i), val) for i, val in enumerate(nest_indices)]
+                # self.solver.ksp.pc.setFieldSplitIS(("0", is_0), ("1", is_1))
+                self.solver.ksp.pc.setFieldSplitIS(*nest_indices_tuples)
+                # 0 == 'additive' [jacobi], 1 == gauss-seidel
+                self.solver.ksp.pc.setFieldSplitType(1)
+                subksps = self.solver.ksp.pc.getFieldSplitSubKSP()
+                for i, subksp in enumerate(subksps):
+                    # subksp.setType('preonly')
+                    # # If there is not diffusion then this is really just a distributed set of ODEs
+                    # if not self._active_compartments[i].has_diffusive_forms:
+                    #     subksp.pc.setType('none')
+                    subksp.setType("preonly")
+                    subksp.pc.setType("hypre")
         else:
             logger.debug(
                 "Using dolfin MixedNonlinearVariationalSolver",
                 extra=dict(format_type="log"),
             )
             self._ubackend = [u[i]._cpp_object for i in range(len(u))]
             self.problem = d.cpp.fem.MixedNonlinearVariationalProblem(
@@ -1112,57 +1200,50 @@
             # self.problem_alternative = d.MixedNonlinearVariationalProblem(Fblock, u, [], J)
             self.solver = d.MixedNonlinearVariationalSolver(self.problem)
 
     # @staticmethod
 
     def get_block_system(self, Fsum, u):
         """
-        The high level dolfin.solve(F==0, u) eventually
+        Modify F and define J in specific structure required
+        for  :code:`dolfin.assemble_mixed()` - use to preassemble linear system
+        for the dolfin MixedNonlinearVariationalSolver (untested)
+
+
+        The high level  :code:`dolfin.solve(F==0, u)` eventually
         calls cpp.fem.MixedNonlinearVariationalSolver,
         but first modifies F and defines J into a specific
-        structure that is required for d.assemble_mixed()
+        structure that is required for  :code:`dolfin.assemble_mixed()`
 
-        ====================================================
-        Comments on d.extract_blocks(F) (which is just a wrapper
+        Comments on :code:`d.extract_blocks(F)` (which is just a wrapper
         around ufl.algorithms.formsplitter)
-        ====================================================
+
         There is some indexing going on behind the scenes, so just
         manually summing what we know to be the
         components of Fblock[0] will not be the same as extract_blocks(F)[0].
         Here is an example:
 
-        F  = sum([f.lhs for f in model.forms]) # single form
-        # first compartment
-        F0 = sum([f.lhs for f in model.forms if f.compartment.name=='cytosol'])
-        Fb0 = extract_blocks(F)[0] # tuple of forms
-
-        F0.equals(Fb0) -> False
-        I0 = F0.integrals()[0].integrand()
-        Ib0 = Fb0.integrals()[0].integrand()
-        # (ufl.Indexed(Argument))) vs ufl.Indexed(ListTensor(ufl.Indexed(Argument)))
-        I0.ufl_operands[0] == Ib0.ufl_operands[0] -> False
-        I0.ufl_operands[1] == Ib0.ufl_operands[1] -> True
-        I0.ufl_operands[0] == Ib0.ufl_operands[0](1) -> True
-        """
-
-        # Fblocks = self.get_block_F(Fsum, u)
-        # Jblocks = self.get_block_J(Fsum, u)
-        # block_sizes = self.get_block_sizes(u)
-        # return Fblocks, Jblocks, block_sizes
+        .. code:: python
+
+            F  = sum([f.lhs for f in model.forms]) # single form
+            # first compartment
+            F0 = sum([f.lhs for f in model.forms if f.compartment.name=='cytosol'])
+            Fb0 = extract_blocks(F)[0] # tuple of forms
+
+            F0.equals(Fb0) -> False
+            I0 = F0.integrals()[0].integrand()
+            Ib0 = Fb0.integrals()[0].integrand()
+            # (ufl.Indexed(Argument))) vs ufl.Indexed(ListTensor(ufl.Indexed(Argument)))
+            I0.ufl_operands[0] == Ib0.ufl_operands[0] -> False
+            I0.ufl_operands[1] == Ib0.ufl_operands[1] -> True
+            I0.ufl_operands[0] == Ib0.ufl_operands[0](1) -> True
+        """
 
-        # =====================================================================
-        # doflin.fem.solving._solve_varproblem()
-        # =====================================================================
         # blocks/partitions are by compartment, not species
         Fblock = d.extract_blocks(Fsum)
-        # J = []
-        # for Fi in Fblock:
-        #     for uj in u:
-        #         dFdu = expand_derivatives(d.derivative(Fi, uj))
-        #         J.append(dFdu)
 
         # =====================================================================
         # doflin.fem.problem.MixedNonlinearVariationalProblem()
         # =====================================================================
         # basically is a wrapper around the cpp class that finalizes preparing
         # F and J into the right format
         # TODO: add dirichlet BCs
@@ -1243,17 +1324,21 @@
 
         global_sizes = [uj.function_space().dim() for uj in u]
 
         # return Flist, Jlist
         return Flist, Jlist, global_sizes
 
     def get_global_sizes(self, u):
+        """Return total number of dof for current model"""
         return [uj.function_space().dim() for uj in u]
 
     def get_block_F(self, Fsum, u):
+        """Assemble block F-vector by compartment
+        (F is the residual)
+        """
         # blocks/partitions are by compartment, not species
         Fblock = d.extract_blocks(Fsum)
 
         # Add in placeholders for empty blocks of F
         if len(Fblock) != len(u):
             Ftemp = [None for i in range(len(u))]
             for Fi in Fblock:
@@ -1287,14 +1372,17 @@
                     else:
                         Fs.append(d.Form(Fsub))
                 Flist.append(Fs)
 
         return Flist
 
     def get_block_J(self, Fsum, u):
+        """Assemble block J by compartment
+        (J is the Jacobian)
+        """
         # blocks/partitions are by compartment, not species
         Fblock = d.extract_blocks(Fsum)
         J = []
         for Fi in Fblock:
             for uj in u:
                 dFdu = expand_derivatives(d.derivative(Fi, uj))
                 J.append(dFdu)
@@ -1325,84 +1413,42 @@
                             extra=dict(format_type="logred"),
                         )
                     Js.append(d.Form(Jsub))
                 Jlist.append(Js)
 
         return Jlist
 
-    # ===============================================================================
-    # Model - Solving
-    # Hierarchy:
-    #
-    # solve():
-    #   - highest level solve. solves over all timesteps
-    # solve_single_timestep()
-    #   - recommended level to solve at. time-loop must be in driver script but
-    #     this allows explicit pre/post processing
-    #     monolithic_solve(), iterative_mpsolve()
-    #   - multiphysics level (for now, we are only considering monolithic formulation)
-    #     newton_solve(), picard_solve()
-    #   - nonlinear level. Only relevant for iterative_mpsolve().
-    #     linear solve
-    #   - For any kind of non-linear problem these should simply be parameters passed
-    #     to the non-linear solver
-    #     (we don't want nonlinear solve implemented at the python level)
-    # ===============================================================================
-    def solve(self, plot_period=1):
-        # Initialize
-        # self.init_solutions_and_plots()
-        # Time loop
-        while True:
-            end_simulation = self.solve_single_timestep(plot_period)
-            if end_simulation:
-                break
-
-    # def solve_single_timestep(self, plot_period=1):
-    #     if self.idx == 0:
-    #         self.stopwatch("Total simulation")
-    #     # Solve using specified multiphysics scheme (just monolithic for now)
-    #     self.monolithic_solve()
-
-    #     # # post processing
-    #     # self.post_process()
-    #     # if (self.idx % plot_period == 0 or self.t >= self.final_t) and plot_period!=0:
-    #     #     self.plot_solution()
-
-    #     # if we've reached final time
-    #     end_simulation = self.t >= self.final_t
-    #     if end_simulation:
-    #         self.stopwatch("Total simulation", stop=True)
-    #         fancy_print(f"Model \'{self.name}\' finished simulating
-    #         (final time = {self.final_t}, {self.idx} time-steps)", format_type='title')
+    def set_form_scaling(self, compartment_name, scaling=1.0, print_scaling=True):
+        for form in self.forms:
+            if form.compartment.name == compartment_name:
+                form.set_scaling(scaling, print_scaling)
 
-    #     return end_simulation
     # ===============================================================================
     # Model - Solving (time related functions)
     # ===============================================================================
     def set_time(self, t):
-        "Explicitly change time"
+        """Explicitly change time"""
         if t != self.t:
             logger.debug(f"Time changed from {self.t} to {t}", extra=dict(format_type="log"))
             self.t = t
             self.T.assign(t)
 
     def set_dt(self, dt):
-        "Explicitly change time-step"
+        """Explicitly change time-step"""
         dt = self.rounded_decimal(dt)
         if self.config.solver["time_precision"] is not None:
             dt = round(dt, self.config.solver["time_precision"])
 
         if dt != self.dt:
             logger.debug(f"dt set to {dt} (previously {self.dt})", extra=dict(format_type="log"))
             self.dt = dt
             self.dT.assign(dt)
 
     def adjust_dt_if_prescribed(self):
-        """
-        Checks to see if the size of a full-time step would pass a "reset dt"
+        """Checks to see if the size of a full-time step would pass a "reset dt"
         checkpoint. At these checkpoints dt is reset to some value
         (e.g. to force smaller sampling during fast events)
         """
         # check that there are reset times specified
         if self.config.solver["adjust_dt"] is None or len(self.config.solver["adjust_dt"]) == 0:
             return
         # Aliases
@@ -1464,45 +1510,62 @@
                     extra=dict(format_type="log_important"),
                 )
                 self.set_dt(new_dt)
                 # set a flag to change dt to the config specified value
                 self.reset_dt = True
 
     def adjust_dt_if_pass_tfinal(self):
-        """
-        Check if current value of t and dt would cause t+dt > t_final
-        """
+        """Check if current value of t and dt would cause t+dt > t_final"""
         tnext = self.t + self.dt
         if tnext > self.final_t:
             new_dt = self.final_t - self.t
             if self.config.solver["time_precision"] is not None:
                 new_dt = round(new_dt, self.config.solver["time_precision"])
             logger.info(
                 f"[{self.idx}, t={self.t}] Adjusting time-step "
                 f"(dt = {self.dt} -> {new_dt}) to avoid passing final time",
                 extra=dict(format_type="log"),
             )
             self.set_dt(new_dt)
 
     def forward_time_step(self):
-        "Take a step forward in time"
+        """Take a step forward in time"""
         self.dt = self.rounded_decimal(self.dt)
         if self.config.solver["time_precision"] is not None:
             self.dt = round(self.dt, self.config.solver["time_precision"])
         self.tn = self.rounded_decimal(self.t)  # save the previous time
         self.t = self.rounded_decimal(self.t + self.dt)
         self.dT.assign(self.dt)
         self.T.assign(self.t)
 
         self.tvec.append(self.t)
         self.dtvec.append(self.dt)
 
         # self.update_time_dependent_parameters()
 
     def monolithic_solve(self):
+        """Solve entire monolithic system using Newton iterations,
+        with the specified PETSc SNES solver
+        (or using the dolfin MixedNonlinearVariationalSolver, untested).
+        If the solver diverges or the solution is negative,
+        this function may call itself to solve the system with
+        a smaller time step if
+
+        .. code:: python
+
+            self.config.solver["attempt_timestep_restart_on_divergence"]
+
+        and/or
+
+        .. code:: python
+
+            self.config.solver["reset_timestep_for_negative_solution"]
+
+        are true.
+        """
         self.idx += 1
         # start a timer for the total time step
         self.stopwatches["Total time step"].start()
         # Adjust dt if necessary (if the last time-step did not
         # converge then it is already adjusted)
         if not self._failed_to_converge:
             # check if there is a manually prescribed time-step size
@@ -1599,15 +1662,16 @@
                 if negVals:
                     self.reset_timestep()
                     # Re-initialize SNES solver
                     if len(self.problem.global_sizes) == 1:
                         self._ubackend = self.u["u"]._functions[0].vector().vec().copy()
                     else:
                         self._ubackend = PETSc.Vec().createNest(
-                            [usub.vector().vec().copy() for usub in self.u["u"]._functions]
+                            [usub.vector().vec().copy() for usub in self.u["u"]._functions],
+                            comm=self.mpi_comm_world,
                         )
                     # need to re-link global function with species-specific functions
                     # after re-setting previous solution
                     self._init_4_4_get_species_u_v_V_dofmaps()
                     self._init_4_5_name_functions()
                     self._failed_to_converge = True
                     self.monolithic_solve()
@@ -1689,17 +1753,15 @@
 
         self.update_solution()  # assign most recently computed solution to "previous solution"
         # self.adjust_dt() # adjusts dt based on number of nonlinear iterations required
         # self.stopwatch("Total time step", stop=True)
         self.stopwatches["Total time step"].stop()
 
     def reset_timestep(self, dt_scale=0.20):
-        """
-        t failed. Revert t->tn. Revert solution
-        """
+        """t failed. Revert t->tn and revert solution"""
         logger.debug(f"Resetting time-step: {self.idx}", extra=dict(format_type="log"))
         # Change t and decrease dt
         self.set_time(self.tvec[-2])  # t=tn
         self.set_dt(float(self.dtvec[-1]) * dt_scale)  # dt=dt*0.2
         # Store information on failed solve
         # idx, idx_nl, idx_l, t, dt, residuals, reason
         self.failed_solves.append(
@@ -1722,77 +1784,89 @@
             self.dtvec,
         ]:  # , self.residuals]:
             data.pop()
         # Undo the solution to the previous time-step
         self.update_solution(ukeys=["u"], unew="n")
 
     def update_time_dependent_parameters(self):
-        r"""Updates all time dependent parameters. Time-dependent parameters are
+        r"""
+        Updates all time dependent parameters. Time-dependent parameters are
         either defined either symbolically or through a data file, and each of
-        these can either be defined as a direct function of t, p(t), or a
-        "pre-integrated expression", \int_{t_n}^{t_{n+1}} P(tau) dtau, which allows for
+        these can either be defined as a direct function of :math:`t, p(t)`, or a
+        "pre-integrated expression", :math:`\int_{t_n}^{t_{n+1}} P(\tau) d\tau`, which allows for
         exact integration when the expression the parameter appears in doesn't rely
         on any other time-dependet variables. This may be useful for guaranteeing
         a certain amount of flux independent of time-stepping.
 
         Backward Euler is essentially making the approximation:
-        du/dt = f(u,t)  ->  (u(t_{n+1}) - u(t_n)) = \int_{t_n}^{t_{n+1}}
-        f(u(t_{n+1}),t_{n+1}) dt \approx dt*f(u(t_{n+1}),t_{n+1})
-        If some portion of f is only dependent on t, e.g. f=f_1+f_2+...+f_n, f_i=f_i(t),
-        we can use the exact expression where F_i(t) is the anti-derivative of f_i(t).
-        \int_{t_n}^{t_{n+1}} f_i(t_{n+1}) -> (F_i(t_{n+1}) - F_i(t_n))
+
+        .. math::
+
+            du/dt = f(u,t)  ->  (u(t_{n+1}) - u(t_n)) = \int_{t_n}^{t_{n+1}}
+            f(u(t_{n+1}),t_{n+1}) dt \approx dt*f(u(t_{n+1}),t_{n+1})
+
+        If some portion of f is only dependent on t, e.g. :math:`f=f_1+f_2+...+f_n, f_i=f_i(t)`,
+        we can use the exact expression where :math:`F_i(t)` is
+        the anti-derivative of :math:`f_i(t)`.
+
+        .. math::
+
+            \int_{t_n}^{t_{n+1}} f_i(t_{n+1}) -> (F_i(t_{n+1}) - F_i(t_n))
 
         Therefore,
-        f(t_{n+1}) = (F_i(t_{n+1}) - F_i(t_n))/dt
+
+        .. math::
+
+            f(t_{n+1}) = (F_i(t_{n+1}) - F_i(t_n))/dt
         """
         # Aliases
         t = float(self.t)
         dt = float(self.dt)
         tn = float(self.tn)
 
         # Update time dependent parameters
         for parameter_name, parameter in self.pc.items:
             new_value = None
             if not parameter.is_time_dependent:
                 continue
             if not parameter.use_preintegration:
                 # Parameters that are defined as dolfin expressions will
                 # automatically be updated by model.T.assign(t)
-                if parameter.type == "expression":
+                if parameter.type == ParameterType.expression:
                     parameter.value = parameter.sym_expr.subs({"t": t}).evalf()
                     parameter.value_vector = np.vstack(
                         (parameter.value_vector, [t, parameter.value])
                     )
                     continue
                 # Parameters from a data file need to have their dolfin constant updated
-                if parameter.type == "from_file":
+                if parameter.type == ParameterType.from_file:
                     t_data = parameter.sampling_data[:, 0]
                     p_data = parameter.sampling_data[:, 1]
                     # We never want time to extrapolate beyond the provided data.
                     if t < t_data[0] or t > t_data[-1]:
                         raise Exception("Parameter cannot be extrapolated beyond provided data.")
                     # Just in case... return a nan if value is outside of bounds
                     new_value = float(np.interp(t, t_data, p_data, left=np.nan, right=np.nan))
                     logger.debug(
                         f"Time-dependent parameter {parameter_name} updated by data. "
                         "New value is {new_value}",
                         extra=dict(format_type="log"),
                     )
 
             if parameter.use_preintegration:
-                if parameter.type == "expression":
+                if parameter.type == ParameterType.expression:
                     a = parameter.preint_sym_expr.subs({"t": tn}).evalf()
                     b = parameter.preint_sym_expr.subs({"t": t}).evalf()
                     new_value = float((b - a) / dt)
                     logger.debug(
                         f"Time-dependent parameter {parameter_name} updated by "
                         "pre-integrated expression. New value is {new_value}",
                         extra=dict(format_type="log"),
                     )
-                if parameter.type == "from_file":
+                if parameter.type == ParameterType.from_file:
                     int_data = parameter.preint_sampling_data
                     a = np.interp(tn, int_data[:, 0], int_data[:, 1], left=np.nan, right=np.nan)
                     b = np.interp(t, int_data[:, 0], int_data[:, 1], left=np.nan, right=np.nan)
                     new_value = float((b - a) / dt)
                     logger.debug(
                         f"Time-dependent parameter {parameter_name} updated by "
                         f"pre-integrated data. New value is {new_value}",
@@ -1805,117 +1879,111 @@
                 parameter.value = new_value
                 parameter.dolfin_constant.assign(new_value)
             else:
                 # Time dependent but nothing assigned
                 raise AssertionError()
 
     def update_solution(self, ukeys=["n"], unew="u"):
-        """
-        After finishing a time step, assign all the most recently computed solutions as
+        """After finishing a time step, assign all the most recently computed solutions as
         the solutions for the previous time step.
         """
         if ukeys is None:
             ukeys = set(self.u.keys()).remove(unew)
 
         for ukey in ukeys:
             if ukey not in self.u.keys():
                 raise ValueError(f"Key {ukey} is not in model.u.keys()")
             # for a function from a mixed function space
             for idx in range(self.num_active_compartments):
                 self.u[ukey].sub(idx).assign(self.u[unew].sub(idx))
 
-    # ===============================================================================
-    # Model - Post-processing
-    # ===============================================================================
-
-    def post_process(self):
-        self.data.compute_statistics(
-            self.u, self.t, self.dt, self.sc, self.pc, self.cc, self.fc, self.nl_idx
-        )
-        self.data.compute_probe_values(self.u, self.sc)
-        self.data.output_pickle()
-        self.data.output_csv()
-
     # =========================================================
     # Model - Data manipulation
     # =========================================================
     # get the values of function u from subspace idx of some
     # mixed function space, V
     @staticmethod
     def dolfin_get_dof_indices(species):  # V, species_idx):
         """
-        Returned indices are *local* to the CPU (not global)
-        function values can be returned e.g.
-        indices = dolfin_get_dof_indices(V,species_idx)
-        u.vector().get_local()[indices]
+        Returns indices *local* to the CPU (not global).
+        Function values can then be returned e.g.
+
+        .. code:: python
+
+            indices = dolfin_get_dof_indices(V,species_idx)
+            u.vector().get_local()[indices]
         """
         if species.dof_map is not None:
             return species.dof_map
         species_idx = species.dof_index
 
         V = sub(species.compartment.V, species_idx, collapse_function_space=False)
 
         indices = np.array(V.dofmap().dofs())
         # indices that this CPU owns
         first_idx, _ = V.dofmap().ownership_range()
 
         return indices - first_idx  # subtract index offset to go from global -> local indices
 
     def dolfin_set_function_values(self, sp, ukey, unew):
-        """
-        d.assign(uold, unew) works when uold is a subfunction
-        uold.assign(unew) does not (it will replace the entire function)
+        """Set values for dolfin function (usually for initial condition)
+        Input unew should either be an expression giving the spatial dependence
+        of u, a constant (float), or a vector of values.
+        :code:`d.assign(uold, unew)` works when uold is a subfunction
+        :code:`uold.assign(unew)` does not (it will replace the entire function)
         """
         if isinstance(unew, d.Expression):
             uinterp = d.interpolate(unew, sp.V)
             d.assign(sp.u[ukey], uinterp)
         elif isinstance(unew, (float, int)):
             uinterp = d.interpolate(d.Constant(unew), sp.V)
             d.assign(sp.u[ukey], uinterp)
-        elif len(unew) > 1:
-            if len(sp.dof_map) == len(unew):
-                # unew is an N x 4 array: [X, Y, Z, function_values]
-                u = self.cc[sp.compartment_name].u[ukey]
-                dof_coord = sp.V.tabulate_dof_coordinates()  # coordinates for the current dof
-                mesh_coord = unew[:, 0:3]  # x,y,z coordinates for initial condition
-                function_values = unew[:, 3]
-                # nearest neighbor interpolation
-                # (in this case, matching up exactly with mesh points)
-                dof_vals_cur = np.zeros((len(mesh_coord),))
-                for i in range(len(dof_coord)):
-                    dist_vec = np.sum((dof_coord[i, :] - mesh_coord) ** 2, axis=1)
-                    dof_vals_cur[i] = function_values[np.argmin(dist_vec)]
-                    if i % 1000 == 0:
-                        logger.debug(f"Set {i} of {len(dof_coord)} function values for {sp.name}")
-                # indices = self.dolfin_get_dof_indices(sp)
-                indices = sp.dof_map
-                uvec = u.vector()
-                values = uvec.get_local()
-                values[indices] = dof_vals_cur
-                uvec.set_local(values)
-                uvec.apply("insert")
+        elif len(sp.dof_map) == len(unew):
+            # unew must be an N x 4 array: [X, Y, Z, function_values]
+            u = self.cc[sp.compartment_name].u[ukey]
+            dof_coord = sp.V.tabulate_dof_coordinates()  # coordinates for the current dof
+            mesh_coord = unew[:, 0:3]  # x,y,z coordinates for initial condition
+            function_values = unew[:, 3]
+            # nearest neighbor interpolation
+            # (in this case, matching up exactly with mesh points)
+            dof_vals_cur = np.zeros((len(mesh_coord),))
+            for i in range(len(dof_coord)):
+                dist_vec = np.sum((dof_coord[i, :] - mesh_coord) ** 2, axis=1)
+                dof_vals_cur[i] = function_values[np.argmin(dist_vec)]
+                if i % 1000 == 0:
+                    logger.debug(f"Set {i} of {len(dof_coord)} function values for {sp.name}")
+            # indices = self.dolfin_get_dof_indices(sp)
+            indices = sp.dof_map
+            uvec = u.vector()
+            values = uvec.get_local()
+            values[indices] = dof_vals_cur
+            uvec.set_local(values)
+            uvec.apply("insert")
         elif isinstance(unew, d.Function):
             logger.debug(f"Function already set for {sp.name}")
         else:
             raise NotImplementedError
 
     @property
     def num_active_compartments(self):
+        """number of compartments with dofs"""
         return len(self._active_compartments)
 
     def get_compartment_residual(self, compartment, norm=None):
+        """returns compartment residual as given norm"""
         res_vec = sum(
             [d.assemble_mixed(form).get_local() for form in self.Fblocks_all[compartment.dof_index]]
         )
         if norm is None:
             return res_vec
         else:
             return np.linalg.norm(res_vec, norm)
 
     def get_total_residual(self, norm=None):
+        """returns total residual for all active compartment as given norm"""
         res_vec = np.hstack(
             [d.assemble_mixed(form).get_local() for form in chain.from_iterable(self.Fblocks_all)]
         )
         res_vec = np.hstack(
             [
                 self.get_compartment_residual(compartment, norm=None)
                 for compartment in self._active_compartments
@@ -1924,24 +1992,29 @@
         assert len(res_vec.shape) == 1
         if norm is None:
             return res_vec
         else:
             return np.linalg.norm(res_vec, norm)
 
     def get_mesh_by_id(self, mesh_id):
+        """returns mesh with id, mesh_id"""
         for mesh in self.parent_mesh.all_meshes.values():
             if mesh.id == mesh_id:
                 return mesh
             else:
                 raise ValueError(f"No mesh with id {mesh_id}")
 
     # ============================================================
     # Model - Printing
     # ============================================================
     def print_meshes(self, tablefmt="fancy_grid"):
+        """Print information associated with child meshes:
+        name, id, dimensionality,
+        num_cells, num_facets, and num_vertices
+        """
         if self.mpi_am_i_root:
             properties_to_print = [
                 "name",
                 "id",
                 "dimensionality",
                 "num_cells",
                 "num_facets",
@@ -1991,8 +2064,9 @@
                     ].num_vertices()
                     tempseries = pandas.Series(tempdict, name=intersection_mesh_name)
                     df = pandas.concat([df, tempseries.to_frame().T], ignore_index=True)
 
             print(tabulate(df, headers="keys", tablefmt=tablefmt))
 
     def rounded_decimal(self, x):
+        """Round time value to specified decimal point"""
         return Decimal(x).quantize(self._base_t)
```

### Comparing `fenics-smart-2.0.1/smart/model_assembly.py` & `fenics-smart-2.1.0/smart/model_assembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-"""
-Classes for parameters, species, compartments, reactions, fluxes, and forms
-Model class contains functions to efficiently solve a system
+"""Classes for parameters, species, compartments, reactions, fluxes, and forms.
+Model class contains functions to efficiently solve a system.
 """
 import dataclasses
 import logging
 import numbers
 import sys
 from collections import OrderedDict as odict
 from dataclasses import dataclass
+from enum import Enum
 from pprint import pformat
 from textwrap import wrap
 from typing import Any, List, Optional, Union
+import warnings
 
 import dolfin as d
 import numpy as np
 import pandas
 import pint
 import sympy as sym
 import ufl
@@ -31,14 +32,15 @@
     "empty_sbmodel",
     "sbmodel_from_locals",
     "Compartment",
     "Parameter",
     "Reaction",
     "Species",
     "sbmodel_from_locals",
+    "ParameterType",
 ]
 
 comm = d.MPI.comm_world
 rank = comm.rank
 size = comm.size
 root = 0
 
@@ -48,18 +50,26 @@
 # ====================================================
 # ====================================================
 # Base Classes
 # ====================================================
 # ====================================================
 
 
+class ParameterType(str, Enum):
+    from_file = "from_file"
+    constant = "constant"
+    expression = "expression"
+
+
+class InvalidObjectException(Exception):
+    pass
+
+
 class ObjectContainer:
-    """
-    Parent class containing general methods used by all "containers"
-    """
+    """Parent class containing general methods used by all "containers" """
 
     def __init__(self, ObjectClass):  # df=None, Dict=None):
         self.Dict = odict()
         self._ObjectClass = ObjectClass
         self.properties_to_print = []  # properties to print
 
     # =====================================================================
@@ -67,49 +77,54 @@
     # ---------------------------------------------------------------------
     # General properties/methods to emulate some dictionary-like structure
     # + add some misc useful structure
     # =====================================================================
 
     @property
     def size(self):
-        "Size of ObjectContainer"
+        """Size of ObjectContainer"""
         return len(self.Dict)
 
     @property
     def items(self):
+        """Return all items in container"""
         return self.Dict.items()
 
     @property
     def values(self):
+        """Return all Dict values"""
         return self.Dict.values()
 
     def __iter__(self):
+        """Iteratively return Dict values"""
         return iter(self.Dict.values())
 
     @property
     def keys(self):
+        """Return all Dict keys"""
         return self.Dict.keys()
 
     @property
     def indices(self):
         return enumerate(self.keys)
 
     def to_dicts(self):
-        "Returns a list of dicts that can be used to recreate the ObjectContainer"
+        """Returns a list of dicts that can be used to recreate the ObjectContainer"""
         return [obj.to_dict() for obj in self.values]
 
     def __getitem__(self, key):
-        "syntactic sugar to allow: objcontainer[key] = objcontainer[key]"
+        """syntactic sugar to allow: :code:`objcontainer[key] = objcontainer[key]`"""
         return self.Dict[key]
 
     def __setitem__(self, key, newvalue):
-        "syntactic sugar to allow: objcontainer[key] = objcontainer[key]"
+        """syntactic sugar to allow: :code:`objcontainer[key] = objcontainer[key]`"""
         self.Dict[key] = newvalue
 
     def add(self, *data):
+        """Add data to object container"""
         if len(data) == 1:
             data = data[0]
             # Adding in the ObjectInstance directly
             if isinstance(data, self._ObjectClass):
                 self[data.name] = data
             # Adding in an iterable of ObjectInstances
             else:
@@ -125,101 +140,99 @@
                     if isinstance(data, dict):
                         for obj_name, obj in data.items():
                             self[obj_name] = obj
                     elif all([isinstance(obj, self._ObjectClass) for obj in data]):
                         for obj in data:
                             self[obj.name] = obj
                     else:
-                        raise Exception("Could not add data to ObjectContainer")
+                        raise InvalidObjectException("Could not add data to ObjectContainer")
         # Adding via ObjectInstance arguments
         else:
             obj = self._ObjectClass(*data)
             self[obj.name] = obj
 
     def remove(self, name):
+        """Remove data from object container"""
         if type(name) != str:
             raise TypeError("Argument must be the name of an object [str] to remove.")
         self.Dict.pop(name)
 
-    # def add_property_to_all(self, property_name, item):
-    #     for obj in self.values:
-    #         setattr(obj, property_name, item)
-
     def get_index(self, idx):
-        """
-        Get an element of the object container ordered dict by referencing its index
-        """
+        """Get an element of the object container ordered dict by referencing its index"""
         return list(self.values)[idx]
 
     # ==============================================================================
-    # ObjectContainer - Internal methods
-    # ------------------------------------------------------------------------------
-    # Mostly methods called by Model.initialize()
-    # ==============================================================================
-
-    # ==============================================================================
     # ObjectContainer - Printing/data-formatting related methods
     # ==============================================================================
 
     def get_pandas_dataframe(
         self, properties_to_print: Optional[List[str]] = None, include_idx: bool = True
     ) -> pandas.DataFrame:
         """
         Create a `pandas.DataFrame` of all items in the class (defined through `self.items`)
 
-        Params:
+        Args:
             properties_to_print: If set only the listed properties (by attribute name)
               is added to the series
-            include_index: If true, add index as the first column in the data-frame..
-
-
-
+            include_index: If true, add index as the first column in the data-frame.
         """
 
         df = pandas.DataFrame()
         if include_idx:
             if properties_to_print is not None and "idx" not in properties_to_print:
                 properties_to_print.insert(0, "idx")
             for idx, (_, instance) in enumerate(self.items):
-                df = pandas.concat(
-                    [
-                        df,
-                        instance.get_pandas_series(properties_to_print=properties_to_print, idx=idx)
-                        .to_frame()
-                        .T,
-                    ]
-                )
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore")
+                    # See https://github.com/hgrecco/pint-pandas/issues/128
+                    df = pandas.concat(
+                        [
+                            df,
+                            instance.get_pandas_series(
+                                properties_to_print=properties_to_print, idx=idx
+                            )
+                            .to_frame()
+                            .T,
+                        ]
+                    )
         else:
             for idx, (_, instance) in enumerate(self.items):
-                df = pandas.concat(
-                    [
-                        df,
-                        instance.get_pandas_series(properties_to_print=properties_to_print)
-                        .to_frame()
-                        .T,
-                    ]
-                )
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore")
+                    # See https://github.com/hgrecco/pint-pandas/issues/128
+                    df = pandas.concat(
+                        [
+                            df,
+                            instance.get_pandas_series(properties_to_print=properties_to_print)
+                            .to_frame()
+                            .T,
+                        ]
+                    )
+
         return df
 
     def print_to_latex(
         self,
         properties_to_print=None,
         max_col_width=None,
         sig_figs=2,
         return_df=True,
     ):
-        """Requires latex packages \siunitx and \longtable"""
+        """
+        Print object properties in latex format.
+        Requires latex packages :code:`\siunitx` and :code:`\longtable`
+        """
 
         df = self.get_pandas_dataframe_formatted(
             properties_to_print=properties_to_print,
             max_col_width=max_col_width,
             sig_figs=sig_figs,
         )
 
-        # Change certain df entries to best format for
+        # Change certain df entries to best format for display
         for col in df.columns:
             # Convert quantity objects to unit
             if isinstance(df[col][0], pint.Quantity):
                 # if tablefmt=='latex':
                 df[col] = df[col].apply(lambda x: f"${x:0.{sig_figs}e~Lx}$")
 
             if col == "idx":
@@ -233,21 +246,23 @@
 
     def get_pandas_dataframe_formatted(
         self,
         properties_to_print: Optional[Union[str, List[str]]] = None,
         max_col_width=50,
         sig_figs=2,
     ):
+        """Get formatted pandas dataframe for printing object properties."""
         # Get the pandas dataframe with the properties we want to print
         if properties_to_print is not None:
             if not isinstance(properties_to_print, list):
                 properties_to_print = [properties_to_print]
         elif hasattr(self, "properties_to_print"):
             properties_to_print = self.properties_to_print
         df = self.get_pandas_dataframe(properties_to_print=properties_to_print, include_idx=False)
+
         if properties_to_print:
             df = df[properties_to_print]
 
         # add new lines to df entries (type str) that exceed max col width
         if max_col_width:
             for col in df.columns:
                 if isinstance(df[col][0], str):
@@ -265,14 +280,16 @@
         self,
         tablefmt="fancy_grid",
         properties_to_print=None,
         filename=None,
         max_col_width=50,
         sig_figs=2,
     ):
+        """Print object properties to file and/or terminal."""
+
         df = self.get_pandas_dataframe_formatted(
             properties_to_print=properties_to_print,
             max_col_width=max_col_width,
             sig_figs=sig_figs,
         )
 
         # # Change certain df entries to best format for printing
@@ -280,15 +297,18 @@
             # Convert quantity objects to unit
             if isinstance(df[col][0], pint.Quantity):
                 # if tablefmt=='latex':
                 df[col] = df[col].apply(lambda x: f"{x:0.{sig_figs}e~P}")
 
         # print to file
         if filename is None:
-            logger.info(tabulate(df, headers="keys", tablefmt=tablefmt))
+            logger.info(
+                tabulate(df, headers="keys", tablefmt=tablefmt),
+                extra=dict(format_type="table"),
+            )
         else:
             original_stdout = sys.stdout  # Save a reference to the original standard output
             with open(filename, "w") as f:  # TODO: Add this to logging
                 # Change the standard output to the file we created.
                 sys.stdout = f
                 print("This message will be written to a file.")
                 print(tabulate(df, headers="keys", tablefmt=tablefmt))  # ,
@@ -298,16 +318,15 @@
         df = self.get_pandas_dataframe(properties_to_print=self.properties_to_print)
         df = df[self.properties_to_print]
 
         return tabulate(df, headers="keys", tablefmt="fancy_grid")
 
 
 class ObjectInstance:
-    """
-    Parent class containing general methods used by all smart
+    """Parent class containing general methods used by all smart
     "objects": i.e. parameters, species, compartments, reactions, fluxes, forms
     """
 
     def _check_input_type_validity(self):
         "Check that the inputs have the same type (or are convertible) to the type hint."
         for field in dataclasses.fields(self):
             value = getattr(self, field.name)
@@ -320,37 +339,35 @@
                     raise TypeError(
                         f"Object {self.name!r} type error: the attribute {field.name!r} "
                         f"is expected to be {field.type}, got {type(value)} instead. "
                         "Conversion to the expected type was attempted but unsuccessful."
                     )
 
     def _convert_pint_quantity_to_unit(self):
-        """
-        Convert all attributes of the class that is a `pint.Quantity` into a `pint.Unit`.
-        """
+        """Convert all attributes of the class that is a :code:`pint.Quantity`
+        into a :code:`pint.Unit`."""
         # strip the magnitude and keep the units. Warn if magnitude!=1
         for name, attr in vars(self).items():
             if isinstance(attr, pint.Quantity):
                 setattr(self, name, quantity_to_unit(attr))
 
     def _convert_pint_unit_to_quantity(self):
-        """
-        Convert all attributes of the class that is a `pint.Unit` into a `pint.Quantity`.
-        """
+        """Convert all attributes of the class that is a :code:`pint.Unit`
+        into a :code:`pint.Quantity`."""
         for name, attr in vars(self).items():
             if isinstance(attr, pint.Unit):
                 setattr(self, name, unit_to_quantity(attr))
 
     def get_pandas_series(
         self, properties_to_print: Optional[List[str]] = None, idx: Optional[int] = None
     ):
         """
-        Convert attributes of the class into a `pandas.Series`.
+        Convert attributes of the class into a :code:`pandas.Series`.
 
-        Params:
+        Args:
             properties_to_print: If set only the listed properties (by attribute name)
                 is added to the series
             index: If set add to series
         """
         if properties_to_print is not None:
             dict_to_convert = odict({"idx": idx})
             dict_to_convert.update(
@@ -363,14 +380,15 @@
                 )
             )
         else:
             dict_to_convert = self.__dict__
         return pandas.Series(dict_to_convert, name=self.name)
 
     def print(self, properties_to_print=None):
+        """Print properties in current object instance."""
         if rank == root:
             logger.info("Name: " + self.name)
             # if a custom list of properties to print is provided, only use those
             if properties_to_print:
                 dict_to_print = dict(
                     [
                         (key, val)
@@ -412,23 +430,86 @@
         for s in self:
             s.quantity
         super().print(tablefmt, self.properties_to_print, filename, max_col_width)
 
 
 @dataclass
 class Parameter(ObjectInstance):
+    """
+    Parameter objects contain information for the various parameters involved in reactions,
+    such as binding rates and dissociation constants.
+    A Parameter object that is constant over time and space is initialized by calling
+
+    .. code:: python
+
+    param_var = Parameter(
+        name, value, unit, group (opt), notes (opt),
+        use_preintegration (opt)
+        )
+
+    Args:
+        name: string naming the parameter
+        value: value of the given parameter
+        unit: units associated with given value
+        group (optional): string placing this parameter in a designated group;
+             for organizational purposes when there are multiple reaction modules
+        notes (optional): string related to this parameter
+        use_preintegration (optional): not applicable for constant parameter
+
+    To initialize a parameter object that varies over time, you can either
+    specify a string that gives the parameter as a function of time (t)
+    or load data from a .txt file.
+
+    To load from a string expression, call:
+
+    .. code:: python
+
+        param_var = Parameter.from_expression(
+            name, sym_expr, unit, preint_sym_expr (opt), group (opt),
+            notes (opt), use_preintegration (opt)
+        )
+
+    Inputs are the same as described above, except:
+
+    Args:
+        sym_expr: string specifying an expression, "t" should be the only free variable
+        preint_sym_expr (optional): string giving the integral of the expression; if not given
+                                  and use_preintegration is true, then sympy tries to integrate
+                                  using sympy.integrate()
+        use_preintegration (optional):  use preintegration in solution process if
+                                     "use_preintegration" is true (defaults to false)
+
+    To load parameter over time from a .txt file, call:
+
+    .. code:: python
+
+        param_var = Parameter.from_file(
+            name, sampling_file, unit, group (opt),
+            notes (opt), use_preintegration (opt)
+        )
+
+    Inputs are the same as described above, except:
+
+    Args:
+        sampling_file: name of text file giving parameter data in two columns (comma-separated) -
+                     first column is time (starting with t=0.0) and second is parameter values
+        use_preintegration (optional):  use preintegration in solution process if
+                                     "use_preintegration" is true (defaults to false),
+                                     uses sci.integrate.cumtrapz for numerical integration
+    """
+
     name: str
     value: float
     unit: pint.Unit
     group: str = ""
     notes: str = ""
     use_preintegration: bool = False
 
     def to_dict(self):
-        "Convert to a dict that can be used to recreate the object."
+        """Convert to a dict that can be used to recreate the object."""
         keys_to_keep = [
             "name",
             "value",
             "unit",
             "group",
             "notes",
             "use_preintegration",
@@ -441,31 +522,83 @@
             "type",
             "free_symbols",
         ]
         return {key: self.__dict__[key] for key in keys_to_keep}
 
     @classmethod
     def from_dict(cls, input_dict):
+        """Read parameter object from Dict"""
         parameter = cls(input_dict["name"], input_dict["value"], input_dict["unit"])
         for key, val in input_dict.items():
             setattr(parameter, key, val)
         parameter.__post_init__()
         return parameter
 
     @classmethod
+    def from_file(cls, name, sampling_file, unit, group="", notes="", use_preintegration=False):
+        """ "
+        Load in a purely time-dependent scalar function from data
+        Data needs to be read in from a text file with two columns
+        where the first column is time (first entry must be 0.0)
+        and the second column is the parameter values.
+        Columns should be comma-separated.
+        """
+        # load in sampling data file
+        sampling_data = np.genfromtxt(sampling_file, dtype="float", delimiter=",")
+        logger.info(f"Loading in data for parameter {name}", extra=dict(format_type="log"))
+        if sampling_data[0, 0] != 0.0 or sampling_data.shape[1] != 2:
+            raise NotImplementedError
+        value = sampling_data[0, 1]  # initial value
+
+        parameter = cls(
+            name,
+            value,
+            unit,
+            group=group,
+            notes=notes,
+            use_preintegration=use_preintegration,
+        )
+
+        if use_preintegration:
+            # preintegrate sampling data using cumtrapz
+            from scipy.integrate import cumtrapz
+
+            int_data = cumtrapz(sampling_data[:, 1], x=sampling_data[:, 0], initial=0)
+            # concatenate time vector
+            preint_sampling_data = np.hstack(
+                sampling_data[:, 0].reshape(-1, 1), int_data.reshape(-1, 1)
+            )
+            parameter.preint_sampling_data = preint_sampling_data
+
+        # initialize instance
+        parameter.sampling_file = sampling_file
+        parameter.sampling_data = sampling_data
+        parameter.is_time_dependent = True
+        parameter.is_space_dependent = False  # not supported yet
+        parameter.type = ParameterType.from_file
+        parameter.__post_init__()
+        logger.info(
+            f"Time-dependent parameter {name} loaded from file.",
+            extra=dict(format_type="log"),
+        )
+
+        return parameter
+
+    @classmethod
     def from_expression(
         cls,
         name,
         sym_expr,
         unit,
         preint_sym_expr=None,
         group="",
         notes="",
         use_preintegration=False,
     ):
+        """Use sympy to parse time-dependent expression for parameter"""
         # Parse the given string to create a sympy expression
         if isinstance(sym_expr, str):
             sym_expr = parse_expr(sym_expr)
         x, y, z = (Symbol(f"x[{i}]") for i in range(3))
         sym_expr = sym_expr.subs({"x": x, "y": y, "z": z})
 
         # Check if expression is time/space dependent
@@ -504,15 +637,15 @@
 
         parameter.free_symbols = free_symbols
         parameter.sym_expr = sym_expr
         parameter.is_time_dependent = is_time_dependent
         parameter.is_space_dependent = is_space_dependent
 
         # parameter.dolfin_expression = d.Expression(sym.printing.ccode(sym_expr), t=0.0, degree=1)
-        parameter.type = "expression"
+        parameter.type = ParameterType.expression
         parameter.__post_init__()
         logger.debug(
             f"Time-dependent parameter {name} evaluated from expression.",
             extra=dict(format_type="log"),
         )
 
         return parameter
@@ -539,23 +672,20 @@
             "free_symbols",
         ]
         for attribute in attributes:
             if not hasattr(self, attribute):
                 setattr(self, attribute, None)
 
         if not hasattr(self, "type"):
-            self.type = "constant"
+            self.type = ParameterType.constant
 
         self._convert_pint_quantity_to_unit()
         self._check_input_type_validity()
         self._convert_pint_unit_to_quantity()
         self.check_validity()
-
-        # self.dolfin_constant = d.Constant(self.value)
-        # self.value_unit = self.value*self.unit
         self.value_vector = np.array([0, self.value])
 
     @property
     def dolfin_quantity(self):
         if hasattr(self, "dolfin_expression") and not self.use_preintegration:
             return self.dolfin_expression * self.unit
         else:
@@ -563,14 +693,15 @@
 
     @property
     def quantity(self):
         self._quantity = self.value * self.unit
         return self._quantity
 
     def check_validity(self):
+        """Confirm that time-dependent parameter is defined in terms of time"""
         if self.is_time_dependent:
             if all(
                 [x in ("", None) for x in [self.sampling_file, self.sym_expr, self.preint_sym_expr]]
             ):
                 raise ValueError(
                     f"Parameter {self.name} is marked as time dependent "
                     "but is not defined in terms of time."
@@ -618,17 +749,42 @@
         else:
             with pandas.option_context("max_colwidth", 1000):
                 logger.info(df.to_latex(escape=False, longtable=True, index=False))
 
 
 @dataclass
 class Species(ObjectInstance):
+    """
+    Each Species object contains information for one state variable in the model
+    (can be a molecule, receptor open probability, membrane voltage, etc.)
+
+    Args:
+        name: string naming the species
+        conc_init: initial concentration for this species
+            (can be an expression given by a string to be parsed by sympy
+            - the only unknowns in the expression should be x, y, and z)
+        conc_units: concentration units for this species
+        D: diffusion coefficient value
+        diffusion_units: units for diffusion coefficient
+        compartment_name: each species should be assigned to a single compartment
+        group (optional): for larger models, specifies a group of species this belongs to;
+            for organizational purposes when there are multiple reaction modules
+
+    Species object is initialized by calling:
+
+    .. code:: python
+
+        species_var = Species(
+            name, initial_condition, concentration_units,
+            D, diffusion_units, compartment_name, group (opt)
+        )
+    """
+
     name: str
     initial_condition: Any
-    # initial_condition: float
     concentration_units: pint.Unit
     D: float
     diffusion_units: pint.Unit
     compartment_name: str
     group: str = ""
 
     def to_dict(self):
@@ -642,14 +798,15 @@
             "compartment_name",
             "group",
         ]
         return {key: self.__dict__[key] for key in keys_to_keep}
 
     @classmethod
     def from_dict(cls, input_dict):
+        """Load Species object from Dict"""
         return cls(**input_dict)
 
     def __post_init__(self):
         # self.sub_species = {} # additional compartments this species
         # may live in in addition to its primary one
         self.is_in_a_reaction = False
         self.is_an_added_species = False
@@ -682,14 +839,20 @@
 
         self._convert_pint_quantity_to_unit()
         self._check_input_type_validity()
         self._convert_pint_unit_to_quantity()
         self.check_validity()
 
     def check_validity(self):
+        """Species validity checks:
+
+        * Initial condition is greater than or equal to 0
+        * Diffusion coefficient is greater than or equal to 0
+        * Diffusion coefficient has units of length^2/time
+        """
         # checking values
         if isinstance(self.initial_condition, float) and self.initial_condition < 0.0:
             raise ValueError(
                 f"Initial condition for species {self.name} must be greater or equal to 0."
             )
         if self.D < 0.0:
             raise ValueError(
@@ -764,14 +927,28 @@
             c.num_dofs_local
             c.num_cells
         super().print(tablefmt, self.properties_to_print, filename, max_col_width)
 
 
 @dataclass
 class Compartment(ObjectInstance):
+    """Each Compartment object contains information describing a surface, volume, or edge
+    within the geometry of interest. The object is initialized by calling:
+
+        .. code:: python
+
+            compartment_var = Compartment(name, dimensionality, compartment_units, cell_marker)
+
+    Args:
+        name: string naming the compartment
+        dimensionality: topological dimensionality (e.g. 3 for volume, 2 for surface)
+        compartment_units: length units for the compartment
+        cell_marker: marker value identifying the compartment in the parent mesh
+    """
+
     name: str
     dimensionality: int
     compartment_units: pint.Unit
     cell_marker: Any
 
     def to_dict(self):
         "Convert to a dict that can be used to recreate the object."
@@ -799,29 +976,34 @@
         self.species = odict()
         self.u = dict()
         self._usplit = dict()
         self.V = None
         self.v = None
 
     def check_validity(self):
+        """
+        Compartment validity checks:
+
+        * Compartment dimensionality is 1,2, or 3
+        * Compartment units are of type "length"
+        """
         if self.dimensionality not in [1, 2, 3]:
             raise ValueError(
                 f"Compartment {self.name} has dimensionality {self.dimensionality}. "
                 "Dimensionality must be in [1,2,3]."
             )
         # checking units
         if not self.compartment_units.check("[length]"):
             raise ValueError(
                 f"Compartment {self.name} has units of {self.compartment_units} "
                 "- units must be dimensionally equivalent to [length]."
             )
 
     def specify_nonadjacency(self, nonadjacent_compartment_list=None):
-        """
-        Specify if this compartment is NOT adjacent to another compartment.
+        """Specify if this compartment is NOT adjacent to another compartment.
         Not necessary, but will speed-up initialization of very large problems.
         Only needs to be specified for surface meshes as those are the
         ones that MeshViews are built on.
         """
         if nonadjacent_compartment_list is None:
             self.nonadjacent_compartment_list = []
         self.nonadjacent_compartment_list = nonadjacent_compartment_list
@@ -837,15 +1019,15 @@
 
     @property
     def dolfin_mesh(self):
         return self.mesh.dolfin_mesh
 
     @property
     def nvolume(self):
-        "nvolume with proper units"
+        """nvolume with proper units"""
         self._nvolume = self.mesh.nvolume * self.compartment_units**self.dimensionality
         return self._nvolume
 
     @property
     def num_cells(self):
         self._num_cells = self.mesh.num_cells
         return self._num_cells
@@ -858,26 +1040,26 @@
     @property
     def num_vertices(self):
         self._num_vertices = self.mesh.num_vertices
         return self._num_vertices
 
     @property
     def num_dofs(self):
-        "Number of degrees of freedom for this compartment"
+        """Number of degrees of freedom for this compartment"""
         # self._num_dofs = self.num_species * self.num_vertices
         # return self._num_dofs
         if self.V is None:
             self._num_dofs = 0
         else:
             self._num_dofs = self.V.dim()
         return self._num_dofs
 
     @property
     def num_dofs_local(self):
-        "Number of degrees of freedom for this compartment, local to this process"
+        """Number of degrees of freedom for this compartment, local to this process"""
         if self.V is None:
             self._num_dofs_local = 0
         else:
             self._ownership_range = self.V.dofmap().ownership_range()
             self._num_dofs_local = self._ownership_range[1] - self._ownership_range[0]
         return self._num_dofs_local
 
@@ -896,14 +1078,67 @@
         max_col_width=50,
     ):
         super().print(tablefmt, self.properties_to_print, filename, max_col_width)
 
 
 @dataclass
 class Reaction(ObjectInstance):
+    """
+    A Reaction object contains information on a single biochemical interaction
+    between species in a single compartment or across multiple compartments.
+
+    Args:
+        name: string naming the reaction
+        lhs: list of strings specifying the reactants for this reaction
+        rhs: list of strings specifying the products for this reaction
+            NOTE: the lists "lhs" and "rhs" determine the stoichiometry of the reaction;
+            for instance, if two A's react to give one B, the reactants list would be
+            :code:`["A","A"]`, and the products list would be :code:`["B"]`
+        param_map: relationship between the parameters specified in the reaction string
+            and those given in the parameter container. By default, the reaction parameters are
+            "on" and "off" when a system obeys simple mass action.
+            If the forward rate is given by a parameter :code:`k1` and the reverse
+            rate is given by :code:`k2`, then :code:`param_map = {"on":"k1", "off":"k2"}`
+        eqn_f_str: For systems not obeying simple mass action,
+            this string specifies the forward reaction rate By default,
+            this string is "on*{all reactants multiplied together}"
+        eqn_r_str: For systems not obeying simple mass action,
+            this string specifies the reverse reaction rate
+            By default, this string is :code:`off*{all products multiplied together}`
+            reaction_type: either "custom" or "mass_action" (default is "mass_action")
+            [never a required argument]
+        species_map: same format as param_map;
+            required if the species does not appear in the lhs or rhs lists
+        explicit_restriction_to_domain: string specifying where the reaction occurs;
+            required if the reaction is not constrained by the reaction string
+            (e.g., if production occurs only at the boundary,
+            but the species being produced exists through the entire volume)
+        group: string placing this reaction in a reaction group;
+            for organizational purposes when there are multiple reaction modules
+            flux_scaling: in certain cases, a given reactant or product
+            may experience a scaled flux (for instance, if we assume that
+            some of the molecules are immediately sequestered after the reaction);
+            in this case, to signify that this flux should be rescaled, we specify
+            :code:`flux_scaling = {scaled_species: scale_factor}`,
+            where scaled_species is a string specifying the species to be scaled and
+            scale_factor is a number specifying the rescaling factor
+
+    .. note::
+
+        The Reaction object is initialized by calling:
+
+        .. code:: python
+
+            reaction_name = Reaction(
+                name, lhs, rhs, param_map,
+                eqn_f_str (opt), eqn_r_str (opt), reaction_type (opt), species_map,
+                explicit_restriction_to_domain (opt), group (opt), flux_scaling (opt)
+            )
+    """
+
     name: str
     lhs: list
     rhs: list
     param_map: dict
     species_map: dict = dataclasses.field(default_factory=dict)
     flux_scaling: dict = dataclasses.field(default_factory=dict)
     reaction_type: str = "mass_action"
@@ -950,14 +1185,22 @@
 
         # Finish initializing the species flux scaling
         for species_name in set(self.lhs + self.rhs):
             if species_name not in self.flux_scaling:
                 self.flux_scaling[species_name] = None
 
     def check_validity(self):
+        """
+        Reaction validity checks:
+
+        * LHS (reactants) and RHS (products) are specified as lists of strings
+        * param_map must be specified as a dict of "str:str"
+        * Species_map must be specified as a dict of "str:str"
+        * If given, flux scaling must be specified as a dict of "species:scale_factor"
+        """
         # Type checking
         if not all([isinstance(x, str) for x in self.lhs]):
             raise TypeError(f"Reaction {self.name} requires a list of strings as input for lhs.")
         if not all([isinstance(x, str) for x in self.rhs]):
             raise TypeError(f"Reaction {self.name} requires a list of strings as input for rhs.")
         if not all([type(k) == str and type(v) == str for (k, v) in self.param_map.items()]):
             raise TypeError(
@@ -979,22 +1222,28 @@
             ):
                 raise TypeError(
                     f"Reaction {self.name} requires a dict of "
                     "str:number as input for flux_scaling."
                 )
 
     def _parse_custom_reaction(self, reaction_eqn_str):
+        "Substitute parameters and species into reaction expression"
         reaction_expr = parse_expr(reaction_eqn_str)
         reaction_expr = reaction_expr.subs(self.param_map)
-        # # use species_scaling if available
-        # reaction_expr = reaction_expr.subs(self._species_scaling_map)
         reaction_expr = reaction_expr.subs(self.species_map)
         return str(reaction_expr)
 
     def reaction_to_fluxes(self):
+        """
+        Convert reactions to fluxes -
+        in general, for each product and each reactant there are two fluxes,
+        one forward flux (dictated by :code:`self.eqn_f_str`)
+        and one reverse flux (dictated by :code:`self.eqn_r_str`),
+        stoichiometry is dictated by the number of times a given species occurs on the lhs or rhs
+        """
         logger.debug(f"Getting fluxes for reaction {self.name}", extra=dict(format_type="log"))
         # set of 2-tuples. (species_name, signed stoichiometry)
         self.species_stoich = {
             (species_name, -1 * self.lhs.count(species_name)) for species_name in self.lhs
         }
         self.species_stoich.update(
             {(species_name, 1 * self.rhs.count(species_name)) for species_name in self.rhs}
@@ -1045,20 +1294,31 @@
             f.assembled_flux
             f.equation_lambda_eval("quantity")
         super().print(tablefmt, self.properties_to_print, filename, max_col_width)
 
 
 @dataclass
 class Flux(ObjectInstance):
+    """Flux objects are created from reaction objects and should not be
+    explicitly initialized by the user.
+    Each flux object contains:
+
+    * name: string (created as reaction name + species name + (f) or (r))
+    * destination_species: flux increases or decreases this species
+    * equation: directionality * stoichiometry * reaction string
+    * reaction: reaction object this flux comes from
+    """
+
     name: str
     destination_species: Species
     equation: sym.Expr
     reaction: Reaction
 
     def check_validity(self):
+        "No validity checks for flux objects currently"
         pass
 
     def __post_init__(self):
         # for nice printing
         self._species_name = self.destination_species.name
 
         self._check_input_type_validity()
@@ -1084,31 +1344,36 @@
         self._post_init_get_integration_measure()
 
         # Check if flux is linear with respect to different components
         self.is_linear_wrt_comp = dict()
         self._post_init_get_is_linear_comp()
 
     def _post_init_get_involved_species_parameters_compartments(self):
+        "Find species, parameters, and compartments involved in this flux"
         self.destination_compartment = self.destination_species.compartment
 
         # Get the subset of species/parameters/compartments that are relevant
         variables = {str(x) for x in self.equation.free_symbols}
         all_params = self.reaction.parameters
         all_species = self.reaction.species
         self.parameters = {x: all_params[x] for x in variables.intersection(all_params.keys())}
         self.species = {x: all_species[x] for x in variables.intersection(all_species.keys())}
         self.compartments = self.reaction.compartments
 
     def _post_init_get_flux_topology(self):
         """
-        Previous flux topology types:
-        [1d] volume:                    PDE of u
-        [1d] surface:                   PDE of v
-        [2d] volume_to_surface:         PDE of v
-        [2d] surface_to_volume:         BC of u
+        "Flux topology" refers to what types of compartments the flux occurs over
+        For instance, if a reaction occurs only in a volume, its topology is type "volume"
+        or if it involves species moving from one volume to another (across a surface),
+        it is of type "volume-surface_to_volume". Depending on the flux topology,
+        the flux will contribute to the system either as a term in the PDE or as
+        a boundary condition.
+
+        The dimensionality indicated in the left brackets below refers to how many
+        compartments are involved in the given flux (e.g. 3d = 3 compartments)
 
         Flux topology types:
         [1d] volume:                    PDE of u
         [1d] surface:                   PDE of v
         [2d] volume_to_surface:         PDE of v
         [2d] surface_to_volume:         BC of u
         [3d] volume-surface_to_volume:  BC of u ()
@@ -1160,14 +1425,28 @@
             self.is_boundary_condition = False
         elif self.topology in ["surface_to_volume", "volume-surface_to_volume"]:
             self.is_boundary_condition = True
         else:
             raise AssertionError()
 
     def _post_init_get_flux_units(self):
+        """
+        Check that flux units match expected type of units.
+        For boundary conditions, the flux units should be
+        (concentration_units / compartment_units) * diffusion_units
+        For fluxes that contribute to the PDE terms, units should be
+        (concentration_units / time)
+        If the units dimensionality does not match the expected form, an error is thrown;
+        if the dimensionality matches, but the units scaling is not 1.0
+        (e.g. if we have a flux specified as nM/s, but concentration_units are defined as uM),
+        then self.unit_scale_factor is set to the appropriate factor
+        (1000 in the example where we need to convert nM -> uM)
+        NOTE: All unit checks are completed using pint, which may not be compatible with
+        certain functions such as sign().
+        """
         concentration_units = self.destination_species.concentration_units
         compartment_units = self.destination_compartment.compartment_units
         diffusion_units = self.destination_species.diffusion_units
 
         # The expected units
         if self.is_boundary_condition:
             self._expected_flux_units = (
@@ -1219,15 +1498,15 @@
                 f"New flux units: {self._expected_flux_units}",
                 extra=dict(new_lines=[0, 1], format_type="log"),
             )
             print("")
 
     def _post_init_get_integration_measure(self):
         """
-        Flux topologys:
+        Flux topologies (cf. definitions in _post_init_get_flux_topology above):
         [1d] volume:                    PDE of u
         [1d] surface:                   PDE of v
         [2d] volume_to_surface:         PDE of v
         [2d] surface_to_volume:         BC of u
         [3d] volume-surface_to_volume:  BC of u ()
         [3d] volume-volume_to_surface:  PDE of v ()
 
@@ -1260,79 +1539,77 @@
         variables = {
             variable.name: variable.dolfin_quantity
             for variable in {**self.parameters, **self.species}.values()
         }
         variables.update({"unit_scale_factor": self.unit_scale_factor})
         return variables
 
-    # @property
-    # def equation_value(self):
-    #     return self.equation_quantity.magnitude
-    # @property
-    # def equation_units(self):
-    #     return unit_to_quantity(self.equation_quantity.units)
-
     def equation_lambda_eval(self, input_type="quantity"):
-        """
-        Evaluates the equation lambda function using either the quantity
+        """Evaluates the equation lambda function using either the quantity
         (value * units), the value, or the units.
         The values and units are evaluated separately and then combined
         because some expressions don't work well
         with pint quantity types.
         """
         # This is an attempt to make the equation lambda work with pint quantities
+        # note - throws an error when it doesn't return a float
+        # (happens when it returns 0 from sign function, for instance)
         self._equation_quantity = self.equation_lambda(**self.equation_variables)
         if input_type == "quantity":
             return self._equation_quantity
         elif input_type == "value":
             return self._equation_quantity.magnitude
         elif input_type == "units":
             return unit_to_quantity(self._equation_quantity.units)
 
     # Seems like setting this as a @property doesn't cause fenics to recompile
 
     @property
     def form(self):
         """-1 factor because terms are defined as if they were on the
-        lhs of the equation F(u;v)=0"""
+        lhs of the equation :math:`F(u;v)=0`"""
         return (
             d.Constant(-1)
             * self.equation_lambda_eval(input_type="value")
             * self.destination_species.v
             * self.measure
         )
 
     @property
     def scalar_form(self):
-        """if the destination species is a vector function,
-        the assembled form will be a vector of size NDOF."""
+        """
+        Defines scalar form for given flux.
+        If the destination species is a vector function,
+        the assembled form will be a vector of size NDOF.
+        """
         return (
             d.Constant(-1)
             * self.equation_lambda_eval(input_type="value")
             * self.destination_species.vscalar
             * self.measure
         )
 
     @property
     def assembled_flux(self):
-        """Same thing as molecules_per_second but doesn't try to convert
-        units (e.g. volumetric concentration is being used on a 2d domain)"""
+        """Attempt to convert flux units to molecules_per_second for printing."""
         try:
             self._assembled_flux = -1 * (
                 d.assemble(self.scalar_form).sum() * self.equation_units * self.measure_units
             ).to(unit.molecule / unit.s)
         except Exception:
             self._assembled_flux = -1 * (
                 d.assemble(self.scalar_form).sum() * self.equation_units * self.measure_units
             )
         return self._assembled_flux
 
     def _post_init_get_is_linear_comp(self):
         """
-        Is the flux linear in terms of a compartment vector (e.g. dj/du['pm'])
+        If the flux is linear in terms of a compartment vector (e.g.
+        :code:`dj/du['pm']`),
+        then sets :code:`self.is_lienar_wrt_comp[comp_name]` to True
         """
         umap = {}
 
         for species_name, species in self.species.items():
             comp_name = species.compartment_name
             umap.update({species_name: "u" + comp_name})
 
@@ -1420,22 +1697,24 @@
     @property
     def integrals(self):
         self._integrals = self.form.integrals()
         return self._integrals
 
 
 def empty_sbmodel():
+    """Initialize empty containers (pc, sc, cc, and rc)"""
     pc = ParameterContainer()
     sc = SpeciesContainer()
     cc = CompartmentContainer()
     rc = ReactionContainer()
     return pc, sc, cc, rc
 
 
 def sbmodel_from_locals(local_values):
+    """Assemble containers from local variables"""
     # FIXME: Add typing
     # Initialize containers
     pc, sc, cc, rc = empty_sbmodel()
     parameters = [x for x in local_values if isinstance(x, Parameter)]
     species = [x for x in local_values if isinstance(x, Species)]
     compartments = [x for x in local_values if isinstance(x, Compartment)]
     reactions = [x for x in local_values if isinstance(x, Reaction)]
```

### Comparing `fenics-smart-2.0.1/smart/solvers.py` & `fenics-smart-2.1.0/smart/solvers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-"""Interface to PETSc SNES solver"""
+"""SMART module interfacing with PETSc SNES solver"""
 import logging
-import os
 from typing import Dict, List, Optional
 
 import dolfin as d
 import petsc4py.PETSc as p
 
 from .common import Stopwatch
 from .model_assembly import Compartment
@@ -17,133 +16,33 @@
     "snes jacobian assemble",
     "snes residual assemble",
     "snes initialize zero matrices",
 ]
 
 
 class smartSNESProblem:
-    """Interface to PETSc SNES solver.
+    """
+    Interface to PETSc SNES solver, defining problem to be solved.
 
     Args:
         u: The function containing the unknown dofs (is a function from a
-            :class:`dolfin.MixedFunctionSpace`)
+            `dolfin.MixedFunctionSpace`)
         Fforms: Nested list of forms for the residual ``F``. Number of
             block rows in the rhs vector is given by the number of items in the outermost list.
         Jforms_all: Nested list of forms for the Jacobian.
-
-            .. note::
-                Number of entries in the outermost list should be ``len(Fforms)**2``
-
-            Flattened such that ``J[i,j]=sum(Jforms_all[i*len(Fforms)+j])``,
+            Number of entries in the outermost list should be ``len(Fforms)**2``
+            flattened such that ``J[i,j]=sum(Jforms_all[i*len(Fforms)+j])``,
             ``i,j=0,..,len(Fforms)-1``.
             The k-th entry of ``Jforms_all`` is a list of forms that are summed up in a given block.
         active_compartments: List of compartments used in the variational form.
-
-            .. note::
-                This input is only used to get the compartment names, should we change the
-                input to only be the names?
         all_compartments: List of all compartments in model.
-
-            .. note::
-                This is only used to get a map from mesh-id to name of compartment.
-                I think we should extract this information
-                from the active compartments.
         stopwatches: Dictionary of stop-watches (stopwatch_name: stopwatch-class).
-
-            .. note::
-                Assumes that one has the entries:
-
-                - ``'snes jacobian assemble'``
-                - ``'snes residual assemble'``
-                - ``'snes initialize zero matrices'``
-        verbose: If True output logger info
-
-    .. note::
-        High-level dolfin solver ``d.solve()`` when applied to Mixed Nonlinear problems:
-        F is the sum of all forms, in smart this is:
-
-        .. highlight:: python
-        .. code-block:: python
-
-            Fsum = sum([f.lhs for f in model.forms]) # single form F0+F1+...+Fn
-            d.solve(Fsum==0, u)
-
-        roughly executes the following:
-
-        .. highlight:: python
-        .. code-block:: python
-
-            d.solve(Fsum==0, u)  # [fem/solving.py]
-            _solve_varproblem()  # [fem/solving.py]
-            eq, ... = _extract_args()
-            # tuple of forms (F0, F1, ..., Fn)
-            F = extract_blocks(eq.lhs) [fem/formmanipulations -> ufl/algorithms/formsplitter]
-            for Fi in F:
-                for uj in u._functions:
-                    Js.append(expand_derivatives(formmanipulations.derivative(Fi, uj)))
-                    # [J00, J01, J02, etc...]
-            problem = MixedNonlinearVariationalProblem(F, u._functions, bcs, Js)
-            solver  = MixedNonlinearVariationalSolver(problem)
-            solver.solve()
-
-        .. highlight:: python
-        .. code-block:: python
-
-            MixedNonlinearVariationalProblem(F, u._functions, bcs, Js)  # [fem/problem.py]
-            u_comps = [u[i]._cpp_object for i in range(len(u))]
-
-            # if len(F)!= len(u) -> Fill empty blocks of F with None
-            # Check that len(J)==len(u)**2 and len(F)==len(u)
-
-            # use F to create Flist. Separate forms by domain:
-            # Flist[i] is a list of Forms separated by domain. E.g. if F1 consists of
-            # integrals on \Omega_1, \Omega_2, and \Omega_3
-            # then Flist[i] is a list with 3 forms
-            If Fi is None -> Flist[i] = cpp.fem.Form(1,0)
-            else -> Flist[i] = [Fi[domain=0], Fi[domain=1], ...]
-
-            # Do the same for J -> Jlist
-            cpp.fem.MixedNonlinearVariationalProblem.__init__(self, Flist, u_comps, bcs, Jlist)
-
-    .. note::
-        .. highlight:: python
-        .. code-block:: python
-
-            # on extract_blocks(F)
-            F  = sum([f.lhs for f in model.forms]) # single form
-            Fb = extract_blocks(F) # tuple of forms
-            Fb0 = Fb[0]
-
-            F0 = sum([f.lhs for f in model.forms if f.compartment.name=='cytosol'])
-            F0.equals(Fb0) -> False
-
-            I0 = F0.integrals()[0].integrand()
-            Ib0 = Fb0.integrals()[0].integrand()
-            (ufl.Indexed(Argument))) vs ufl.Indexed(ListTensor(ufl.Indexed(Argument)))
-            I0.ufl_operands[0] == Ib0.ufl_operands[0] -> False
-            I0.ufl_operands[1] == Ib0.ufl_operands[1] -> True
-            I0.ufl_operands[0] == Ib0.ufl_operands[0](1) -> True
-
-        ``V.__repr__()`` shows the UFL coordinate element (finite element over coordinate
-        vector field) and finite element of the function space. We can access individually with:
-
-        .. highlight:: python
-        .. code-block:: python
-
-            V.ufl_domain().ufl_coordinate_element()
-            V.ufl_element()
-
-            # on assembler
-            d.fem.assembling.assemble_mixed(form, tensor)
-            assembler = cpp.fem.MixedAssembler()
-
-            fem.assemble.cpp/assemble_mixed(GenericTensor& A, const Form& a, bool add)
-            MixedAssembler assembler;
-            assembler.add_values = add;
-            assembler.assemble(A, a);
+            Must include at least `snes jacobian assemble`, `snes residual assemble`
+            and `snes initialize zero matrices`
+        verbose: If True, output logger info.
     """
 
     def __init__(
         self,
         u: d.Function,
         Fforms: List[List[d.Form]],
         Jforms_all: List[List[d.Form]],
@@ -180,50 +79,32 @@
             (z[::block_size] / block_size).astype("int32")
             for z, block_size in zip(self.lgmaps, self.block_sizes)
         ]
         self.lgmaps_petsc = [
             p.LGMap().create(lgmap, bsize=bsize, comm=self.comm)
             for bsize, lgmap in zip(self.block_sizes, self.lgmaps)
         ]
-        # self.blgmaps_petsc = [p.LGMap().create(blgmap, bsize=bsize, comm=self.comm)
-        # for bsize, blgmap in zip(self.block_sizes, self.block_indices)] # block version
 
         self.local_ownership_ranges = [V.dofmap().ownership_range() for V in self.W]
         self.local_sizes = [x[1] - x[0] for x in self.local_ownership_ranges]
         self.global_sizes = [V.dim() for V in self.W]
 
         # Need sizes because some forms may be empty
-        # self.local_sizes = [c._num_dofs_local for c in active_compartments]
-        # self.global_sizes = [c._num_dofs for c in active_compartments]
         self.is_single_domain = len(self.global_sizes) == 1
-
         self.active_compartment_names = [c.name for c in active_compartments]
         self.mesh_id_to_name = {c.mesh_id: c.name for c in all_compartments}
 
         # Should we print assembly info (can get very verbose)
         self.verbose = verbose
 
         # Timings
         for key in _stopwatch_keys:
             if key not in stopwatches.keys():
                 raise ValueError(f"Stopwatch dictionary missing stopwatch {key}")
         self.stopwatches = stopwatches
-        # Our custom assembler (something about dolfin's init_global_tensor was not
-        # correct so we manually initialize the petsc matrix and then wrap with dolfin)
-        # This assembly routine is the exact same as d.assemble_mixed() except
-        # init_global_tensor() is commented out
-        # Thanks to Prof. Kamensky and his student for the idea
-        # https://github.com/hanzhao2020/PENGoLINS/blob/main/PENGoLINS/cpp/transfer_matrix.cpp
-        os.path.dirname(os.path.realpath(__file__))
-        # cpp_file = open(path_to_script_dir+"/cpp/MixedAssemblerTemp.cpp","r")
-        # cpp_code = cpp_file.read()
-        # cpp_file.close()
-        # self.module = d.compile_cpp_code(cpp_code,include_dirs=[path_to_script_dir+"/cpp",])
-        # self.assembler = d.compile_cpp_code(cpp_code,include_dirs=[path_to_script_dir+"/cpp",]).
-        # MixedAssemblerTemp()
 
         # Check for empty forms
         self.empty_forms = []
         for i in range(self.dim):
             for j in range(self.dim):
                 ij = i * self.dim + j
                 if all(
@@ -267,15 +148,17 @@
                     logger.debug(
                         f"cpu {self.rank}: (ijk)={(i,j,k)} "
                         f"({self.local_sizes[i]}, {self.local_sizes[j]}, "
                         f"{self.global_sizes[i]}, {self.global_sizes[j]})",
                         extra=dict(format_type="log"),
                     )
 
-                    d.assemble_mixed(Jforms[ij][k], tensor=self.tensors[ij][k])
+                    d.assemble_mixed(
+                        Jforms[ij][k], tensor=self.tensors[ij][k]
+                    )  # causes issues when running multiple meshes in parallel
 
                 if non_empty_forms == 0:
                     # If all forms are empty, we don't need to assemble. Initialize to zero matrix
                     if self.verbose:
                         logger.debug(
                             f"{self.Jijk_name(i,j)} is empty - initializing as "
                             f"empty PETSc Matrix with local size {self.local_sizes[i]}, "
@@ -333,15 +216,15 @@
                     if self.verbose:
                         logger.warning(
                             f"{self.Fjk_name(j,k)}] has no function space",
                             extra=dict(format_type="log"),
                         )
                     continue
 
-                tensor = d.PETScVector()
+                tensor = d.PETScVector(self.comm)
 
                 if Fsum is None:
                     Fsum = d.assemble_mixed(self.Fforms[j][k], tensor=tensor)
                 else:
                     # Fsum.axpy(1, d.assemble_mixed(self.Fforms[j][k], tensor=tensor).vec(),
                     # structure=Fsum.Structure.DIFFERENT_NONZERO_PATTERN)
                     Fsum += d.assemble_mixed(self.Fforms[j][k], tensor=tensor)
@@ -358,26 +241,25 @@
 
             Fpetsc.append(Fsum.vec())
 
         if self.is_single_domain:
             # We can't use a nest vector
             self.Fpetsc_nest = d.PETScVector(Fpetsc[0]).vec()
         else:
-            self.Fpetsc_nest = p.Vec().createNest(Fpetsc)
+            self.Fpetsc_nest = p.Vec().createNest(Fpetsc, comm=self.comm)
         self.Fpetsc_nest.assemble()
 
     def assemble_Jnest(self, Jnest):
-        """Assemble Jacobian nest matrix
+        """Assemble Jacobian nest matrix.
+
+        Args:
+            Jnest : petsc4py.Mat
+                PETSc nest matrix representing the Jacobian
 
-        Parameters
-        ----------
-        Jnest : petsc4py.Mat
-            PETSc nest matrix representing the Jacobian
 
-        Jmats are created using assemble_mixed(Jform) and are dolfin.PETScMatrix types
         """
         if self.verbose:
             logger.debug("Assembling block Jacobian", extra=dict(format_type="assembly"))
         self.stopwatches["snes jacobian assemble"].start()
         dim = self.dim
 
         Jform = self.Jforms_all
@@ -446,14 +328,21 @@
                 self.print_Jijk_info(i, j, k=None, tensor=Jij_petsc)
 
         Jnest.assemble()
 
         self.stopwatches["snes jacobian assemble"].pause()
 
     def assemble_Fnest(self, Fnest):
+        """
+        Assemble residual nest vector
+
+        Arguments:
+            Fnest : petsc4py.Vec
+                PETSc nest vector representing the residual
+        """
         dim = self.dim
         if self.verbose:
             logger.debug("Assembling block residual vector", extra=dict(format_type="assembly"))
         self.stopwatches["snes residual assemble"].start()
 
         if self.is_single_domain:
             Fj_petsc = [Fnest]
@@ -490,21 +379,21 @@
         self.assemble_Fnest(Fnest)
 
     def J(self, snes, u, Jnest, P):
         self.copy_u(u)
         self.assemble_Jnest(Jnest)
 
     def init_petsc_matrix(self, i, j, nnz_guess=None, set_lgmap=False, assemble=False):
-        """Initialize a PETSc matrix with appropriate structure
+        """
+        Initialize a PETSc matrix with appropriate structure
 
-        Parameters
-        ----------
-        i,j : indices of the block
-        nnz_guess : number of non-zeros (per row) to guess for the matrix
-        assemble : whether to assemble the matrix or not
+        Args:
+            i,j : indices of the block
+            nnz_guess : number of non-zeros (per row) to guess for the matrix
+            assemble : whether to assemble the matrix or not (Boolean)
         """
         self.stopwatches["snes initialize zero matrices"].start()
 
         M = p.Mat().create(comm=self.comm)
         # ((local_nrows, global_nrows), (local_ncols, global_ncols))
         M.setSizes(
             (
@@ -532,37 +421,35 @@
         self.stopwatches["snes initialize zero matrices"].pause()
 
         return M
 
     def init_petsc_vector(self, j, assemble=False):
         """Initialize a dolfin wrapped PETSc vector with appropriate structure
 
-        Parameters
-        ----------
-        j : index
-        assemble : whether to assemble the vector or not
+        Args:
+            j : index
+            assemble : whether to assemble the vector or not (Boolean)
         """
         V = p.Vec().create(comm=self.comm)
         V.setSizes((self.local_sizes[j], self.global_sizes[j]))
         V.setUp()
         # V.setLGMap(self.lgmaps_petsc[j])
 
         if assemble:
             V.assemble()
         return V
 
     def Jijk_name(self, i: int, j: int, k: Optional[int] = None):
-        """
-        Get a string representation of an entry of the Jacobian.
+        """Get a string representation of an entry of the Jacobian.
 
         Args:
             i: Row index
             j: Column index
             k: If the Jacobian entry is a sum of forms, get the name
-                of the domain in the `k`th entry.
+                of the domain in the k'th entry.
         """
         if k is None:
             return (
                 f"J{i}{j} = dF[{self.active_compartment_names[i]}]"
                 f"/du[{self.active_compartment_names[j]}]"
             )
         else:
@@ -578,27 +465,28 @@
 
     def Fjk_name(self, j: int, k: Optional[int] = None):
         """
         Get a string representation of an entry of the residual.
 
         Args:
             j: Block index
-            k: If the residual entry is a sum of forms, get the name
-                of the domain in the `k`th entry.
+            k: If the residual entry is a sum of forms, get the
+                name of the domain in the k'th entry.
         """
 
         if k is None:
             return f"F{j} = F[{self.active_compartment_names[j]}]"
         else:
             if (num_entries := len(self.Fforms[j])) <= k:
                 raise RuntimeError(f"F[{j}] only consists of {num_entries} componets")
             domain_name = self.mesh_id_to_name[self.Fforms[j][k].function_space(0).mesh().id()]
             return f"F{j} = F[{self.active_compartment_names[j]}] (domain={domain_name})"
 
     def print_Jijk_info(self, i, j, k=None, tensor=None):
+        "Print information on Jacobian nest matrix"
         if not self.verbose:
             return
         if tensor is None:
             return
         # Print some useful info on Jijk
         info = tensor.getInfo()
         # , block_size={int(info['block_size'])}
@@ -621,15 +509,16 @@
         if info["nz_unneeded"] > 0:
             logger.warning(
                 f"WARNING: {info['nz_unneeded']} nonzero entries are unneeded",
                 extra=dict(format_type="warning"),
             )
 
     def get_csr_matrix(self, i, j):
-        "This is a matrix that can be used to visualize the sparsity pattern using plt.spy()"
+        """This is a matrix that can be used to visualize
+        the sparsity pattern using :code:`plt.spy()`"""
         if self.is_single_domain:
             M = self.Jpetsc_nest
         else:
             M = self.Jpetsc_nest.getNestSubMatrix(i, j)
         from scipy.sparse import csr_matrix
 
         return csr_matrix(M.getValuesCSR()[::-1], shape=M.size)
```

### Comparing `fenics-smart-2.0.1/smart/units.py` & `fenics-smart-2.1.0/smart/units.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.0.1/smart/utils.py` & `fenics-smart-2.1.0/smart/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Converts a json_str (either a string of the json itself, or a filepath to
     the json) to the appropriate data type (given by a string).
 
     Args:
         json_file: Path to json file
         data_type: Type of container, either parameter, species, compartment or reaction.
 
-    ..note:
+    .. note::
         Several abbreviations of the above are allowed, see source code for details
 
     """
     json_file = Path(json_file)
     if json_file.suffix != ".json":
         raise ValueError("Invalid suffix for {json_file}, expected '.json'")
     if not json_file.exists():
```

### Comparing `fenics-smart-2.0.1/tests/test_species.py` & `fenics-smart-2.1.0/tests/test_species.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 import math
 
 import pytest
 
 import smart
 
 
-@pytest.fixture(name="A_kwargs")
-def example_species():
-    kwargs = dict(
-        concentration_units=smart.units.unit.uM,
-        diffusion_units=smart.units.unit.um**2 / smart.units.unit.sec,
-        initial_condition=0.01,
-        D=2.0,
-        name="A",
-        compartment_name="Cyto",
-        group="Some group",
-    )
-
-    A = smart.model_assembly.Species(**kwargs)
-    return (A, kwargs)
-
-
-def test_Species_initialization(A_kwargs):
-    A, kwargs = A_kwargs
-    assert A.name == kwargs["name"]
-    assert A.latex_name == kwargs["name"]
-    assert str(A.sym) == kwargs["name"]
+def test_Species_initialization(species_kwargs_A):
+    """Test that we can initialize a SpeciesContainer"""
+    A = smart.model_assembly.Species(**species_kwargs_A)
+    assert A.name == species_kwargs_A["name"]
+    assert A.latex_name == species_kwargs_A["name"]
+    assert str(A.sym) == species_kwargs_A["name"]
 
-    assert math.isclose(A.initial_condition, kwargs["initial_condition"])
+    assert math.isclose(A.initial_condition, species_kwargs_A["initial_condition"])
     assert (
-        A.initial_condition_quantity == kwargs["initial_condition"] * kwargs["concentration_units"]
+        A.initial_condition_quantity
+        == species_kwargs_A["initial_condition"] * species_kwargs_A["concentration_units"]
     )
-    assert A.concentration_units == smart.units.unit_to_quantity(kwargs["concentration_units"])
-    assert math.isclose(A.D, kwargs["D"])
-    assert A.diffusion_units == smart.units.unit_to_quantity(kwargs["diffusion_units"])
-    assert A.D_quantity == kwargs["D"] * kwargs["diffusion_units"]
+    assert A.concentration_units == smart.units.unit_to_quantity(
+        species_kwargs_A["concentration_units"]
+    )
+    assert math.isclose(A.D, species_kwargs_A["D"])
+    assert A.diffusion_units == smart.units.unit_to_quantity(species_kwargs_A["diffusion_units"])
+    assert A.D_quantity == species_kwargs_A["D"] * species_kwargs_A["diffusion_units"]
 
-    assert A.compartment_name == kwargs["compartment_name"]
-    assert A.group == kwargs["group"]
+    assert A.compartment_name == species_kwargs_A["compartment_name"]
+    assert A.group == species_kwargs_A["group"]
     assert A.dof_map is None
     assert A.ut is None
     assert A.v is None
     assert A.u == {}
     assert A.is_an_added_species is False
     assert A.is_in_a_reaction is False
 
 
-@pytest.mark.xfail
-def test_access_vscalar(A_kwargs):
-    A, kwargs = A_kwargs
-    # We should have proper error handling here
-    A.vscalar
-
-
-@pytest.mark.xfail
-def test_access_dolfin_quatity(A_kwargs):
-    A, kwargs = A_kwargs
-    # We should have proper error handling here
-    A.dolfin_quantity
+def test_SpeciesContainer(species_kwargs_A, species_kwargs_AER):
+    """Test that we can initialize a SpeciesContainer"""
+    A = smart.model_assembly.Species(**species_kwargs_A)
+    AER = smart.model_assembly.Species(**species_kwargs_AER)
+    sc = smart.model_assembly.SpeciesContainer()
+    assert sc.size == 0
+    sc.add([A])
+    assert sc.size == 1
+    sc["A"] == A
+    sc.add([A])
+    # Adding same species should not do anything
+    assert sc.size == 1
+    sc.add([AER])
+    assert sc.size == 2
+    assert set(sc.keys) == {"A", "AER"}
+
+
+def test_add_non_Species_to_SpeciesContainer_raises_InvalidObjectException(
+    compartment_kwargs_Cyto,
+):
+    """Test that if we try to add something different than a species
+    to a SpeciesContainer then an exception will be raised"""
+    sc = smart.model_assembly.SpeciesContainer()
+    Cyto = smart.model_assembly.Compartment(**compartment_kwargs_Cyto)
+    with pytest.raises(smart.model_assembly.InvalidObjectException):
+        sc.add([Cyto])
```

