# Comparing `tmp/odetoolbox-2.5-py3-none-any.whl.zip` & `tmp/odetoolbox-2.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 49541 bytes, number of entries: 18
--rw-r--r--  2.0 unx    18311 b- defN 22-Oct-13 08:24 odetoolbox/__init__.py
--rw-r--r--  2.0 unx     8906 b- defN 22-Oct-13 08:24 odetoolbox/analytic_integrator.py
--rw-r--r--  2.0 unx     2710 b- defN 22-Oct-13 08:00 odetoolbox/dependency_graph_plotter.py
--rw-r--r--  2.0 unx     3146 b- defN 22-Oct-13 08:00 odetoolbox/integrator.py
--rw-r--r--  2.0 unx    21610 b- defN 22-Oct-13 08:00 odetoolbox/mixed_integrator.py
--rw-r--r--  2.0 unx     1601 b- defN 22-Oct-13 08:00 odetoolbox/plot_helper.py
--rw-r--r--  2.0 unx    29650 b- defN 22-Oct-13 08:24 odetoolbox/shapes.py
--rw-r--r--  2.0 unx     6310 b- defN 22-Oct-13 08:24 odetoolbox/singularity_detection.py
--rw-r--r--  2.0 unx     3774 b- defN 22-Oct-13 08:24 odetoolbox/spike_generator.py
--rw-r--r--  2.0 unx     9190 b- defN 22-Oct-13 08:00 odetoolbox/stiffness.py
--rw-r--r--  2.0 unx     2262 b- defN 22-Oct-13 08:00 odetoolbox/sympy_printer.py
--rw-r--r--  2.0 unx    17439 b- defN 22-Oct-13 08:24 odetoolbox/system_of_shapes.py
--rwxr-xr-x  2.0 unx     4320 b- defN 22-Oct-13 08:32 odetoolbox-2.5.data/scripts/ode_analyzer.py
--rw-r--r--  2.0 unx    17941 b- defN 22-Oct-13 08:32 odetoolbox-2.5.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1757 b- defN 22-Oct-13 08:32 odetoolbox-2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-13 08:32 odetoolbox-2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Oct-13 08:32 odetoolbox-2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1519 b- defN 22-Oct-13 08:32 odetoolbox-2.5.dist-info/RECORD
-18 files, 150549 bytes uncompressed, 47059 bytes compressed:  68.7%
+Zip file size: 50204 bytes, number of entries: 19
+-rw-r--r--  2.0 unx    17764 b- defN 23-Jun-13 14:58 odetoolbox/__init__.py
+-rw-r--r--  2.0 unx     8906 b- defN 23-Jun-13 14:58 odetoolbox/analytic_integrator.py
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jun-13 14:58 odetoolbox/config.py
+-rw-r--r--  2.0 unx     2810 b- defN 23-Jun-13 14:58 odetoolbox/dependency_graph_plotter.py
+-rw-r--r--  2.0 unx     3146 b- defN 23-Jun-13 14:58 odetoolbox/integrator.py
+-rw-r--r--  2.0 unx    21676 b- defN 23-Jun-13 14:58 odetoolbox/mixed_integrator.py
+-rw-r--r--  2.0 unx     1601 b- defN 23-Jun-13 14:58 odetoolbox/plot_helper.py
+-rw-r--r--  2.0 unx    28633 b- defN 23-Jun-13 14:58 odetoolbox/shapes.py
+-rw-r--r--  2.0 unx     6310 b- defN 23-Jun-13 14:58 odetoolbox/singularity_detection.py
+-rw-r--r--  2.0 unx     3795 b- defN 23-Jun-13 14:58 odetoolbox/spike_generator.py
+-rw-r--r--  2.0 unx     9199 b- defN 23-Jun-13 14:58 odetoolbox/stiffness.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Jun-13 14:58 odetoolbox/sympy_helpers.py
+-rw-r--r--  2.0 unx    16643 b- defN 23-Jun-13 14:58 odetoolbox/system_of_shapes.py
+-rwxr-xr-x  2.0 unx     3822 b- defN 23-Jun-13 15:03 odetoolbox-2.5.1.data/scripts/ode_analyzer.py
+-rw-r--r--  2.0 unx    17941 b- defN 23-Jun-13 15:03 odetoolbox-2.5.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1759 b- defN 23-Jun-13 15:03 odetoolbox-2.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 15:03 odetoolbox-2.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 15:03 odetoolbox-2.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1608 b- defN 23-Jun-13 15:03 odetoolbox-2.5.1.dist-info/RECORD
+19 files, 150460 bytes uncompressed, 47582 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: odetoolbox/__init__.py
 Comment: 
 
 Filename: odetoolbox/analytic_integrator.py
 Comment: 
 
+Filename: odetoolbox/config.py
+Comment: 
+
 Filename: odetoolbox/dependency_graph_plotter.py
 Comment: 
 
 Filename: odetoolbox/integrator.py
 Comment: 
 
 Filename: odetoolbox/mixed_integrator.py
@@ -24,32 +27,32 @@
 
 Filename: odetoolbox/spike_generator.py
 Comment: 
 
 Filename: odetoolbox/stiffness.py
 Comment: 
 
-Filename: odetoolbox/sympy_printer.py
+Filename: odetoolbox/sympy_helpers.py
 Comment: 
 
 Filename: odetoolbox/system_of_shapes.py
 Comment: 
 
-Filename: odetoolbox-2.5.data/scripts/ode_analyzer.py
+Filename: odetoolbox-2.5.1.data/scripts/ode_analyzer.py
 Comment: 
 
-Filename: odetoolbox-2.5.dist-info/LICENSE.md
+Filename: odetoolbox-2.5.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: odetoolbox-2.5.dist-info/METADATA
+Filename: odetoolbox-2.5.1.dist-info/METADATA
 Comment: 
 
-Filename: odetoolbox-2.5.dist-info/WHEEL
+Filename: odetoolbox-2.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: odetoolbox-2.5.dist-info/top_level.txt
+Filename: odetoolbox-2.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odetoolbox-2.5.dist-info/RECORD
+Filename: odetoolbox-2.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odetoolbox/__init__.py

```diff
@@ -16,33 +16,32 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with NEST.  If not, see <http://www.gnu.org/licenses/>.
 #
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
-from .sympy_printer import SympyPrinter, _is_zero
-from .system_of_shapes import SystemOfShapes
-from .shapes import MalformedInputException, Shape
-
-import copy
 import json
 import logging
 import sys
-
 import sympy
 from sympy.core.expr import Expr as SympyExpr   # works for both sympy 1.4 and 1.8
 
+from .config import Config
+from .sympy_helpers import SympyPrinter, _is_zero, _is_sympy_type
+from .system_of_shapes import SystemOfShapes
+from .shapes import MalformedInputException, Shape
+
 
 try:
     import pygsl.odeiv as odeiv
     PYGSL_AVAILABLE = True
 except ImportError as ie:
-    logging.warn("PyGSL is not available. The stiffness test will be skipped.")
-    logging.warn("Error when importing: " + str(ie))
+    logging.warning("PyGSL is not available. The stiffness test will be skipped.")
+    logging.warning("Error when importing: " + str(ie))
     PYGSL_AVAILABLE = False
 
 if PYGSL_AVAILABLE:
     from .stiffness import StiffnessTester
 
 try:
     import graphviz
@@ -51,90 +50,77 @@
     PLOT_DEPENDENCY_GRAPH = False
 
 if PLOT_DEPENDENCY_GRAPH:
     from .dependency_graph_plotter import DependencyGraphPlotter
 
 sympy.Basic.__str__ = lambda self: SympyPrinter().doprint(self)
 
-default_config = {
-    "input_time_symbol": "t",
-    "output_timestep_symbol": "__h",
-    "differential_order_symbol": "__d",
-    "sim_time": 100E-3,
-    "max_step_size": 999.,
-    "integration_accuracy_abs": 1E-6,
-    "integration_accuracy_rel": 1E-6
-}
 
-
-def _dependency_analysis(shape_sys, shapes, differential_order_symbol, parameters=None):
+def _dependency_analysis(shape_sys, shapes, parameters=None):
     r"""
     Perform dependency analysis and plot dependency graph.
     """
     logging.info("Dependency analysis...")
     dependency_edges = shape_sys.get_dependency_edges()
-    node_is_lin = shape_sys.get_lin_cc_symbols(dependency_edges, differential_order_symbol=differential_order_symbol, parameters=parameters)
+    node_is_lin = shape_sys.get_lin_cc_symbols(dependency_edges, parameters=parameters)
     if PLOT_DEPENDENCY_GRAPH:
         DependencyGraphPlotter.plot_graph(shapes, dependency_edges, node_is_lin, fn="/tmp/ode_dependency_graph_before.dot")
     node_is_lin = shape_sys.propagate_lin_cc_judgements(node_is_lin, dependency_edges)
     if PLOT_DEPENDENCY_GRAPH:
         DependencyGraphPlotter.plot_graph(shapes, dependency_edges, node_is_lin, fn="/tmp/ode_dependency_graph.dot")
     return dependency_edges, node_is_lin
 
 
-def _read_global_config(indict, default_config):
+def _read_global_config(indict):
     r"""
     Process global configuration options.
     """
     logging.info("Processing global options...")
-    options_dict = copy.deepcopy(default_config)
     if "options" in indict.keys():
         for key, value in indict["options"].items():
-            assert key in default_config.keys(), "Unknown key specified in global options dictionary: \"" + str(key) + "\""
-            options_dict[key] = value
-
-    return options_dict
+            assert key in Config.config.keys(), "Unknown key specified in global options dictionary: \"" + str(key) + "\""
+            Config.config[key] = value
 
 
-def _from_json_to_shapes(indict, options_dict, parameters=None) -> List[Shape]:
+def _from_json_to_shapes(indict, parameters=None) -> Tuple[List[Shape], Dict[sympy.Symbol, str]]:
     r"""
     Process the input, construct Shape instances.
 
     :param indict: ODE-toolbox input dictionary.
-    :param options_dict: ODE-toolbox global configuration dictionary.
     """
 
     logging.info("Processing input shapes...")
     shapes = []
     # first run for grabbing all the variable names. Coefficients might be incorrect.
     all_variable_symbols = []
     all_parameter_symbols = set()
     all_variable_symbols_ = set()
     for shape_json in indict["dynamics"]:
-        shape = Shape.from_json(shape_json, time_symbol=options_dict["input_time_symbol"], differential_order_symbol=options_dict["differential_order_symbol"], parameters=parameters)
+        shape = Shape.from_json(shape_json, parameters=parameters)
         all_variable_symbols.extend(shape.get_state_variables())
-        all_variable_symbols_.update(shape.get_state_variables(derivative_symbol="__d"))
+        all_variable_symbols_.update(shape.get_state_variables(derivative_symbol=Config().differential_order_symbol))
         all_parameter_symbols.update(set(shape.reconstitute_expr().free_symbols))
     all_parameter_symbols -= all_variable_symbols_
     del all_variable_symbols_
+    assert all([_is_sympy_type(sym) for sym in all_variable_symbols])
     logging.info("All known variables: " + str(all_variable_symbols) + ", all parameters used in ODEs: " + str(all_parameter_symbols))
 
     for param in all_parameter_symbols:
         if parameters is None:
             parameters = dict()
 
         assert isinstance(param, SympyExpr)
         if not param in parameters.keys():
             # this parameter was used in an ODE, but not explicitly numerically specified
             logging.info("No numerical value specified for parameter \"" + str(param) + "\"")    # INFO level because this is OK!
             parameters[param] = None
 
     # second run with the now-known list of variable symbols
     for shape_json in indict["dynamics"]:
-        shape = Shape.from_json(shape_json, all_variable_symbols=all_variable_symbols, time_symbol=options_dict["input_time_symbol"], parameters=parameters, _debug=True)
+        shape = Shape.from_json(shape_json, all_variable_symbols=all_variable_symbols, parameters=parameters, _debug=True)
         shapes.append(shape)
 
     return shapes, parameters
 
 
 def _find_variable_definition(indict, name: str, order: int) -> Optional[str]:
     r"""Find the definition (as a string in the input dictionary) of variable named ``name`` with order ``order``, and return it as a string. Return None if a definition by that name and order could not be found."""
@@ -166,35 +152,36 @@
             name, order, rhs = Shape._parse_defining_expression(expr)
             if order == 1:
                 variable_names.append(name)
 
     return variable_names
 
 
-def _analysis(indict, disable_stiffness_check: bool = False, disable_analytic_solver: bool = False, preserve_expressions: Union[bool, Iterable[str]] = False, simplify_expression: str = "sympy.simplify(expr)", log_level: Union[str, int] = logging.WARNING) -> Tuple[List[Dict], SystemOfShapes, List[Shape]]:
+def _analysis(indict, disable_stiffness_check: bool = False, disable_analytic_solver: bool = False, preserve_expressions: Union[bool, Iterable[str]] = False, simplify_expression: Optional[str] = None, log_level: Union[str, int] = logging.WARNING) -> Tuple[List[Dict], SystemOfShapes, List[Shape]]:
     r"""
     Like analysis(), but additionally returns ``shape_sys`` and ``shapes``.
 
     For internal use only!
     """
 
     # import sys;sys.setrecursionlimit(max(sys.getrecursionlimit(), 10000))
 
-    global default_config
-
     _init_logging(log_level)
 
     logging.info("Analysing input:")
     logging.info(json.dumps(indict, indent=4, sort_keys=True))
 
     if "dynamics" not in indict:
         logging.info("Warning: empty input (no dynamical equations found); returning empty output")
         return [], SystemOfShapes.from_shapes([]), []
 
-    options_dict = _read_global_config(indict, default_config)
+    _read_global_config(indict)
+
+    if simplify_expression:
+        Config.config["simplify_expression"] = simplify_expression
 
     # copy parameters from the input and make sure keys are of type sympy.Symbol
     parameters = None
     if "parameters" in indict.keys():
         parameters = {}
         for k, v in indict["parameters"].items():
             if type(k) is str:
@@ -203,23 +190,23 @@
                 assert type(k) is sympy.Symbol
                 parameters[k] = v
 
     #
     #   create Shapes and SystemOfShapes
     #
 
-    shapes, parameters = _from_json_to_shapes(indict, options_dict, parameters=parameters)
+    shapes, parameters = _from_json_to_shapes(indict, parameters=parameters)
 
     for shape in shapes:
         if not shape.is_homogeneous() and shape.order > 1:
             logging.error("For symbol " + str(shape.symbol) + ": higher-order inhomogeneous ODEs are not supported")
             sys.exit(1)
 
     shape_sys = SystemOfShapes.from_shapes(shapes, parameters=parameters)
-    dependency_edges, node_is_lin = _dependency_analysis(shape_sys, shapes, differential_order_symbol=options_dict["differential_order_symbol"], parameters=parameters)
+    dependency_edges, node_is_lin = _dependency_analysis(shape_sys, shapes, parameters=parameters)
 
 
     #
     #   generate analytical solutions (propagators) where possible
     #
 
     solvers_json = []
@@ -233,29 +220,28 @@
     for i in range(shape_sys.A_.shape[0]):
         if not _is_zero(shape_sys.b_[i]) and shape_sys.shape_order_from_system_matrix(i) > 1:
             analytic_syms = [sym for sym in analytic_syms if not sym in shape_sys.get_connected_symbols(i)]
 
     if analytic_syms:
         logging.info("Generating propagators for the following symbols: " + ", ".join([str(k) for k in analytic_syms]))
         sub_sys = shape_sys.get_sub_system(analytic_syms)
-        analytic_solver_json = sub_sys.generate_propagator_solver(output_timestep_symbol=options_dict["output_timestep_symbol"])
+        analytic_solver_json = sub_sys.generate_propagator_solver()
         analytic_solver_json["solver"] = "analytical"
         solvers_json.append(analytic_solver_json)
 
 
     #
     #   generate numerical solvers for the remainder
     #
 
     if len(analytic_syms) < len(shape_sys.x_):
         numeric_syms = list(set(shape_sys.x_) - set(analytic_syms))
         logging.info("Generating numerical solver for the following symbols: " + ", ".join([str(sym) for sym in numeric_syms]))
         sub_sys = shape_sys.get_sub_system(numeric_syms)
-        solver_json = sub_sys.generate_numeric_solver(state_variables=shape_sys.x_,
-                                                      simplify_expression=simplify_expression)
+        solver_json = sub_sys.generate_numeric_solver(state_variables=shape_sys.x_)
         solver_json["solver"] = "numeric"   # will be appended to if stiffness testing is used
         if not disable_stiffness_check:
             if not PYGSL_AVAILABLE:
                 raise Exception("Stiffness test requested, but PyGSL not available")
 
             logging.info("Performing stiffness test...")
             kwargs = {}   # type: Dict[str, Any]
@@ -264,16 +250,16 @@
                 assert random_seed >= 0, "Random seed needs to be a non-negative integer"
                 kwargs["random_seed"] = random_seed
             if "parameters" in indict.keys():
                 kwargs["parameters"] = indict["parameters"]
             if "stimuli" in indict.keys():
                 kwargs["stimuli"] = indict["stimuli"]
             for key in ["sim_time", "max_step_size", "integration_accuracy_abs", "integration_accuracy_rel"]:
-                if "options" in indict.keys() and key in options_dict.keys():
-                    kwargs[key] = float(options_dict[key])
+                if "options" in indict.keys() and key in Config().keys():
+                    kwargs[key] = float(Config()[key])
             if not analytic_solver_json is None:
                 kwargs["analytic_solver_dict"] = analytic_solver_json
             tester = StiffnessTester(sub_sys, shapes, **kwargs)
             solver_type = tester.check_stiffness()
             if not solver_type is None:
                 solver_json["solver"] += "-" + solver_type
                 logging.info(solver_type + " scheme")
@@ -284,18 +270,18 @@
     #
     #   copy the initial values from the input to the output for convenience; convert to numeric values
     #
 
     for solver_json in solvers_json:
         solver_json["initial_values"] = {}
         for shape in shapes:
-            all_shape_symbols = [str(sympy.Symbol(str(shape.symbol) + options_dict["differential_order_symbol"] * i)) for i in range(shape.order)]
+            all_shape_symbols = [str(sympy.Symbol(str(shape.symbol) + Config().differential_order_symbol * i)) for i in range(shape.order)]
             for sym in all_shape_symbols:
                 if sym in solver_json["state_variables"]:
-                    solver_json["initial_values"][sym] = str(shape.get_initial_value(sym.replace(options_dict["differential_order_symbol"], "'")))
+                    solver_json["initial_values"][sym] = str(shape.get_initial_value(sym.replace(Config().differential_order_symbol, "'")))
 
 
     #
     #   copy the parameter values from the input to the output for convenience; convert into numeric values
     #
 
     if "parameters" in indict.keys():
@@ -338,21 +324,25 @@
                 raise MalformedInputException("Requested to preserve expression of variable \"" + preserve_expressions_var + "\", but it was not defined as a first-order ODE")
     else:
         raise MalformedInputException("``preserve_expressions`` parameter should be either a boolean or a list of strings corresponding to variable names")
 
     for solver_json in solvers_json:
         if "update_expressions" in solver_json.keys():
             for sym, expr in solver_json["update_expressions"].items():
+                solver_json["update_expressions"][sym] = str(expr)
+
                 if preserve_expressions and sym in preserve_expressions:
+                    if "analytic" in solver_json["solver"]:
+                        logging.warning("Not preserving expression for variable \"" + sym + "\" as it is solved by propagator solver")
+                        continue
+
                     logging.info("Preserving expression for variable \"" + sym + "\"")
                     var_def_str = _find_variable_definition(indict, sym, order=1)
                     assert var_def_str is not None
-                    solver_json["update_expressions"][sym] = var_def_str.replace("'", options_dict["differential_order_symbol"])
-                else:
-                    solver_json["update_expressions"][sym] = str(expr)
+                    solver_json["update_expressions"][sym] = var_def_str.replace("'", Config().differential_order_symbol)
 
         if "propagators" in solver_json.keys():
             for sym, expr in solver_json["propagators"].items():
                 solver_json["propagators"][sym] = str(expr)
 
     logging.info("In ode-toolbox: returning outdict = ")
     logging.info(json.dumps(solvers_json, indent=4, sort_keys=True))
@@ -367,15 +357,15 @@
     :param log_level: Sets the logging threshold. Logging messages which are less severe than ``log_level`` will be ignored. Log levels can be provided as an integer or string, for example "INFO" (more messages) or "WARN" (fewer messages). For a list of valid logging levels, see https://docs.python.org/3/library/logging.html#logging-levels
     """
     fmt = '%(levelname)s:%(message)s'
     logging.basicConfig(format=fmt)
     logging.getLogger().setLevel(log_level)
 
 
-def analysis(indict, disable_stiffness_check: bool = False, disable_analytic_solver: bool = False, preserve_expressions: Union[bool, Iterable[str]] = False, simplify_expression: str = "sympy.simplify(expr)", log_level: Union[str, int] = logging.WARNING) -> List[Dict]:
+def analysis(indict, disable_stiffness_check: bool = False, disable_analytic_solver: bool = False, preserve_expressions: Union[bool, Iterable[str]] = False, simplify_expression: Optional[str] = None, log_level: Union[str, int] = logging.WARNING) -> List[Dict]:
     r"""
     The main entry point of the ODE-toolbox API.
 
     :param indict: Input dictionary for the analysis. For details, see https://ode-toolbox.readthedocs.io/en/master/#input
     :param disable_stiffness_check: Whether to perform stiffness checking.
     :param disable_analytic_solver: Set to True to return numerical solver recommendations, and no propagators, even for ODEs that are analytically tractable.
     :param preserve_expressions: Set to True, or a list of strings corresponding to individual variable names, to disable internal rewriting of expressions, and return same output as input expression where possible. Only applies to variables specified as first-order differential equations.
```

## odetoolbox/dependency_graph_plotter.py

```diff
@@ -17,14 +17,16 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with NEST.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import logging
 
+from .config import Config
+
 
 class DependencyGraphPlotter:
     r"""
     Use graphviz to plot a dependency graph between state variables.
     """
 
     @classmethod
@@ -36,15 +38,16 @@
         :param dependency_edges: List of edges returned from dependency analysis.
         :param node_is_lin: List of Booleans returned from dependency analysis.
         :param fn: Filename to write PNG image as.
         """
 
         from graphviz import Digraph
 
-        E = [(str(sym1).replace("__d", "'"), str(sym2).replace("__d", "'")) for sym1, sym2 in dependency_edges]
+        E = [(str(sym1).replace(Config().differential_order_symbol, "'"),
+              str(sym2).replace(Config().differential_order_symbol, "'")) for sym1, sym2 in dependency_edges]
 
         dot = Digraph(comment="Dependency graph", engine="dot", format="pdf")
         dot.attr(compound="true")
         nodes = []
         for shape in shapes:
             if node_is_lin[shape.symbol]:
                 style = "filled"
```

## odetoolbox/mixed_integrator.py

```diff
@@ -26,26 +26,28 @@
 import numpy.random
 import os
 import sympy
 import sympy.utilities.autowrap
 from sympy.utilities.autowrap import CodeGenArgumentListError
 import time
 
+
 from .analytic_integrator import AnalyticIntegrator
+from .config import Config
 from .integrator import Integrator
 from .plot_helper import import_matplotlib
 from .shapes import Shape
-from .sympy_printer import _is_sympy_type
+from .sympy_helpers import _is_sympy_type
 
 try:
     import pygsl.odeiv as odeiv
     PYGSL_AVAILABLE = True
 except ImportError as ie:
-    logging.warn("PyGSL is not available. The stiffness test will be skipped.")
-    logging.warn("Error when importing: " + str(ie))
+    logging.warning("PyGSL is not available. The stiffness test will be skipped.")
+    logging.warning("Error when importing: " + str(ie))
     PYGSL_AVAILABLE = False
 
 
 class ParametersIncompleteException(Exception):
     """
     Thrown in case not all parameters are assigned a numerical value before integration was attempted.
     """
@@ -103,15 +105,15 @@
         self.analytic_integrator = None
         self._update_expr = self._system_of_shapes.generate_numeric_solver()["update_expressions"].copy()
         self._update_expr_wrapped = {}
 
         self.all_variable_symbols = list(self._system_of_shapes.x_)
         if not self.analytic_solver_dict is None:
             self.all_variable_symbols += self.analytic_solver_dict["state_variables"]
-        self.all_variable_symbols = [sympy.Symbol(str(sym).replace("'", "__d")) for sym in self.all_variable_symbols]
+        self.all_variable_symbols = [sympy.Symbol(str(sym).replace("'", Config().differential_order_symbol)) for sym in self.all_variable_symbols]
 
         for sym, expr in self._update_expr.items():
             try:
                 self._update_expr_wrapped[sym] = sympy.utilities.autowrap.autowrap(expr.subs(self._locals),
                                                                                    args=self.all_variable_symbols,
                                                                                    backend="cython",
                                                                                    helpers=Shape._sympy_autowrap_helpers)
@@ -262,15 +264,15 @@
                         y_log.append(y)
 
                     if h_suggested < h_requested:     # ignore small requested step sizes; look only at actually obtained step sizes
                         h_min = min(h_min, h_suggested)
 
                     if h_min < h_min_lower_bound:
                         estr = "Integration step below %.e (s=%.f). Please check your ODE." % (h_min_lower_bound, h_min)
-                        logging.warn(estr)
+                        logging.warning(estr)
                         if raise_errors:
                             raise Exception(estr)
 
                     h_sum += h_suggested
                     n_timesteps_taken += 1
```

## odetoolbox/shapes.py

```diff
@@ -14,43 +14,47 @@
 # useful, but WITHOUT ANY WARRANTY; without even the implied warranty
 # of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with NEST.  If not, see <http://www.gnu.org/licenses/>.
 #
+
+from __future__ import annotations
+
 from typing import List, Mapping, Tuple
 
 import functools
 import logging
 import re
 import sympy
 import sympy.parsing.sympy_parser
 
 from sympy.core.expr import Expr as SympyExpr   # works for both sympy 1.4 and 1.8
 from sympy.core.numbers import One as SympyOne
 from sympy.core.numbers import Zero as SympyZero
 
-from .sympy_printer import _is_sympy_type, _is_zero
+from .config import Config
+from .sympy_helpers import _custom_simplify_expr, _is_sympy_type, _is_zero
 
 
 class MalformedInputException(Exception):
     """
     Thrown in case an error occurred while processing malformed input.
     """
     pass
 
 
 def is_constant_term(term, parameters: Mapping[sympy.Symbol, str] = None):
     r"""
     :return: :python:`True` if and only if this term contains only numerical values and parameters; :python:`False` otherwise.
     """
-    assert all([type(k) is sympy.Symbol for k in parameters.keys()])
     if parameters is None:
         parameters = {}
+    assert all([type(k) is sympy.Symbol for k in parameters.keys()])
     return type(term) in [sympy.Float, sympy.Integer, SympyZero, SympyOne] \
         or all([sym in parameters.keys() for sym in term.free_symbols])
 
 
 class Shape:
     r"""
     This class provides a canonical representation of a shape function independently of the way in which the user specified the shape. It assumes a differential equation of the general form (where bracketed superscript :math:`{}^{(n)}` indicates the :math:`n`-th derivative with respect to time):
@@ -66,16 +70,14 @@
     ::
 
        x''' = c0 + c1*x + c2*x' + c3*x'' + x*y + x**2
 
     the :python:`symbol` of the ODE would be :python:`x` (i.e. without any qualifiers), :python:`order` would be 3, :python:`derivative_factors` would contain the linear part in the form of the list :python:`[c1, c2, c3]`, the inhomogeneous term would be :python:`c0` and the nonlinear part :python:`x*y + x**2` is stored in :python:`nonlin_term`.
     """
 
-    EXPRESSION_SIMPLIFICATION_THRESHOLD = 1000
-
     # a minimal subset of sympy classes and functions to avoid "from sympy import *"
     _sympy_globals = {"Symbol": sympy.Symbol,
                       "Integer": sympy.Integer,
                       "Float": sympy.Float,
                       "Function": sympy.Function,
                       "Pow": sympy.Pow,
                       "power": sympy.Pow,
@@ -101,15 +103,15 @@
                       "DiracDelta": sympy.DiracDelta}
 
     # cython backend (used by sympy autowrap()) cannot handle these functions; need to provide alternative implementation
     _sympy_autowrap_helpers = [("Min", (abs(sympy.symbols("x") + sympy.symbols("y")) - abs(sympy.symbols("x") - sympy.symbols("y"))) / 2, [sympy.symbols("x"), sympy.symbols("y")]),
                                ("Max", (abs(sympy.symbols("x") + sympy.symbols("y")) + abs(sympy.symbols("x") - sympy.symbols("y"))) / 2, [sympy.symbols("x"), sympy.symbols("y")]),
                                ("Heaviside", (sympy.symbols("x") + abs(sympy.symbols("x"))) / (2 * abs(sympy.symbols("x")) + 1E-300), [sympy.symbols("x")])]
 
-    def __init__(self, symbol, order, initial_values, derivative_factors, inhom_term=sympy.Float(0.), nonlin_term=sympy.Float(0.), lower_bound=None, upper_bound=None, derivative_symbol="__d", debug=False):
+    def __init__(self, symbol, order, initial_values, derivative_factors, inhom_term=sympy.Float(0.), nonlin_term=sympy.Float(0.), lower_bound=None, upper_bound=None):
         r"""
         Perform type and consistency checks and assign arguments to member variables.
 
         :param symbol: Symbolic name of the shape without additional qualifiers like prime symbols or similar.
         :param order: Order of the ODE representing the shape.
         :param initial_values: Initial values of the ODE representing the shape. The dict contains :python:`order` many key-value pairs: one for each derivative that occurs in the ODE. The keys are strings created by concatenating the variable symbol with as many single quotation marks (') as the derivation order. The values are SymPy expressions.
         :param derivative_factors: The factors for the derivatives that occur in the ODE. This list has to contain :path:`order` many values, i.e. one for each derivative that occurs in the ODE. The values have to be in ascending order, i.e. :python:`[c1, c2, c3]` for the given example.
@@ -143,45 +145,35 @@
                 raise MalformedInputException("Initial value specified for unknown variable \"" + str(iv_basename) + "\" in differential equation for variable \"" + str(symbol) + "\"")
             if differential_order >= self.order:
                 raise MalformedInputException("Initial value \"" + str(iv_name) + "\" specifies initial value for degree " + str(differential_order) + ", which is too high in order-" + str(self.order) + " differential equation")
 
         self.initial_values = initial_values
 
         for sym in initial_values.keys():
-            if derivative_symbol in str(sym):
-                raise MalformedInputException("Input variable name \"" + str(sym) + "\" should not contain the string \"" + derivative_symbol + "\", which is used to indicate variable differential order")
+            if Config().differential_order_symbol in str(sym):
+                raise MalformedInputException("Input variable name \"" + str(sym) + "\" should not contain the string \"" + Config().differential_order_symbol + "\", which is used to indicate variable differential order")
 
         if not len(derivative_factors) == order:
             raise MalformedInputException(str(len(derivative_factors)) + " derivative factors specified, while " + str(order) + " were expected based on differential equation definition")
 
         for df in derivative_factors:
             if not _is_sympy_type(df):
                 raise MalformedInputException("Derivative factor \"%r\" is not a SymPy expression" % df)
 
         self.derivative_factors = derivative_factors
-
-        if len(str(inhom_term)) > Shape.EXPRESSION_SIMPLIFICATION_THRESHOLD:
-            logging.warning("Shape \"" + str(self.symbol) + "\" initialised with an expression that exceeds SymPy simplification threshold")
-            self.inhom_term = inhom_term
-        else:
-            self.inhom_term = sympy.simplify(inhom_term)
-
-        if len(str(nonlin_term)) > Shape.EXPRESSION_SIMPLIFICATION_THRESHOLD:
-            logging.warning("Shape \"" + str(self.symbol) + "\" initialised with an expression that exceeds SymPy simplification threshold")
-            self.nonlin_term = nonlin_term
-        else:
-            self.nonlin_term = sympy.simplify(nonlin_term)
+        self.inhom_term = _custom_simplify_expr(inhom_term)
+        self.nonlin_term = _custom_simplify_expr(nonlin_term)
 
         self.lower_bound = lower_bound
         if not self.lower_bound is None:
-            self.lower_bound = sympy.simplify(self.lower_bound)
+            self.lower_bound = _custom_simplify_expr(self.lower_bound)
 
         self.upper_bound = upper_bound
         if not self.upper_bound is None:
-            self.upper_bound = sympy.simplify(self.upper_bound)
+            self.upper_bound = _custom_simplify_expr(self.upper_bound)
 
         logging.debug("Created Shape with symbol " + str(self.symbol) + ", derivative_factors = " + str(self.derivative_factors) + ", inhom_term = " + str(self.inhom_term) + ", nonlin_term = " + str(self.nonlin_term))
 
 
     def __str__(self):
         s = "Shape \"" + str(self.symbol) + "\" of order " + str(self.order)
         return s
@@ -282,23 +274,21 @@
         symbol = symbol_match.group()
 
         order = len(re.findall("'", lhs))
         return symbol, order, rhs
 
 
     @classmethod
-    def from_json(cls, indict, all_variable_symbols=None, time_symbol=sympy.Symbol("t"), differential_order_symbol="__d", parameters=None, _debug=False):
+    def from_json(cls, indict, all_variable_symbols=None, parameters=None, _debug=False):
         r"""
         Create a :python:`Shape` instance from an input dictionary.
 
         :param indict: Input dictionary, i.e. one element of the :python:`"dynamics"` list supplied in the ODE-toolbox input dictionary.
         :param all_variable_symbols: All known variable symbols. :python:`None` or list of string.
-        :param time_symbol: sympy Symbol representing the independent time variable.
         :param parameters: An optional dictionary of parameters to their defining expressions.
-        :param differential_order_symbol: String used for identifying differential order. XXX: only :python:`"__d"` is supported for now.
         """
         if not "expression" in indict:
             raise MalformedInputException("No `expression` keyword found in input")
 
         if not indict["expression"].count("=") == 1:
             raise MalformedInputException("Expecting exactly one \"=\" symbol in defining expression: \"" + str(indict["expression"]) + "\"")
 
@@ -347,27 +337,25 @@
             lower_bound = indict["lower_bound"]
 
         upper_bound = None
         if "upper_bound" in indict.keys():
             upper_bound = indict["upper_bound"]
 
         if order == 0:
-            return Shape.from_function(symbol, rhs, differential_order_symbol=differential_order_symbol)
-        else:
-            return Shape.from_ode(symbol, rhs, initial_values, all_variable_symbols=all_variable_symbols, lower_bound=lower_bound, upper_bound=upper_bound, differential_order_symbol=differential_order_symbol, parameters=parameters)
+            return Shape.from_function(symbol, rhs)
+
+        return Shape.from_ode(symbol, rhs, initial_values, all_variable_symbols=all_variable_symbols, lower_bound=lower_bound, upper_bound=upper_bound, parameters=parameters)
 
 
-    def reconstitute_expr(self, derivative_symbol: str = "__d") -> SympyExpr:
+    def reconstitute_expr(self) -> SympyExpr:
         r"""
         Recreate right-hand side expression from internal representation (linear coefficients, inhomogeneous, and nonlinear parts).
-
-        :param differential_order_symbol: String used for identifying differential order. XXX: only :python:`"__d"` is supported for now.
         """
         expr = self.inhom_term + self.nonlin_term
-        derivative_symbols = self.get_state_variables(derivative_symbol=derivative_symbol)
+        derivative_symbols = self.get_state_variables(derivative_symbol=Config().differential_order_symbol)
         for derivative_factor, derivative_symbol in zip(self.derivative_factors, derivative_symbols):
             expr += derivative_factor * derivative_symbol
         logging.info("Shape " + str(self.symbol) + ": reconstituting expression " + str(expr))
         return expr
 
 
     @staticmethod
@@ -421,55 +409,53 @@
         logging.debug("\tinhomogeneous term: " + str(inhom_term))
         logging.debug("\tnonlinear term: " + str(nonlin_term))
 
         return lin_factors, inhom_term, nonlin_term
 
 
     @classmethod
-    def from_function(cls, symbol: str, definition, max_t=100, max_order=4, all_variable_symbols=None, time_symbol=sympy.Symbol("t"), differential_order_symbol=sympy.Symbol("__d"), debug=False):
+    def from_function(cls, symbol: str, definition, max_t=100, max_order=4, all_variable_symbols=None, debug=False) -> Shape:
         r"""
         Create a Shape object given a function of time.
 
         Only functions of time that have a homogeneous ODE equivalent are supported (inhomogeneous ODE functions are not supported).
 
         For a complete description of the algorithm, see https://ode-toolbox.readthedocs.io/en/latest/index.html#converting-direct-functions-of-time
 
         :param symbol: The variable name of the shape (e.g. :python:`"alpha"`, :python:`"I"`)
         :param definition: The definition of the shape (e.g. :python:`"(e/tau_syn_in) * t *  exp(-t/tau_syn_in)"`)
         :param all_variable_symbols: All known variable symbols. :python:`None` or list of string.
 
         :return: The canonical representation of the postsynaptic shape
-        :rtype: Shape
 
         :Example:
 
         >>> Shape.from_function("I_in", "(e/tau) * t * exp(-t/tau)")
         """
 
         if all_variable_symbols is None:
             all_variable_symbols = []
 
         all_variable_symbols_dict = {str(el): el for el in all_variable_symbols}
 
-        symbol = sympy.Symbol(symbol)
         definition = sympy.parsing.sympy_parser.parse_expr(definition, global_dict=Shape._sympy_globals, local_dict=all_variable_symbols_dict)
 
         # `derivatives` is a list of all derivatives of `shape` up to the order we are checking, starting at 0.
-        derivatives = [definition, sympy.diff(definition, time_symbol)]
+        derivatives = [definition, sympy.diff(definition, Config().input_time_symbol)]
 
-        logging.info("\nProcessing function-of-time shape \"" + str(symbol) + "\" with defining expression = \"" + str(definition) + "\"")
+        logging.info("\nProcessing function-of-time shape \"" + symbol + "\" with defining expression = \"" + str(definition) + "\"")
 
 
         #
         #   to avoid a division by zero below, we have to find a `t` so that the shape function is not zero at this `t`.
         #
 
         t_val = None
         for t_ in range(0, max_t):
-            if not _is_zero(definition.subs(time_symbol, t_)):
+            if not _is_zero(definition.subs(Config().input_time_symbol, t_)):
                 t_val = t_
                 break
 
         logging.debug("Found t: " + str(t_val))
 
         if t_val is None:
 
@@ -485,46 +471,46 @@
         #   first handle the case for an ODE of order 1, i.e. of the form I' = a0 * I
         #
 
         order = 1
 
         logging.debug("\tFinding ode for order 1...")
 
-        derivative_factors = [(1 / derivatives[0] * derivatives[1]).subs(time_symbol, t_val)]
+        derivative_factors = [(1 / derivatives[0] * derivatives[1]).subs(Config().input_time_symbol, t_val)]
         diff_rhs_lhs = derivatives[1] - derivative_factors[0] * derivatives[0]
-        found_ode = _is_zero(sympy.simplify(diff_rhs_lhs))
+        found_ode = _is_zero(diff_rhs_lhs)
 
 
         #
         #   If `shape` does not satisfy a linear homogeneous ODE of order 1, we try to find one of higher order in a loop. The loop runs while no linear homogeneous ODE was found and the maximum order to check for was not yet reached.
         #
 
         while not found_ode and order < max_order:
             order += 1
 
             logging.debug("\tFinding ode for order " + str(order) + "...")
 
             # Add the next higher derivative to the list
-            derivatives.append(sympy.diff(derivatives[-1], time_symbol))
+            derivatives.append(sympy.diff(derivatives[-1], Config().input_time_symbol))
 
             X = sympy.zeros(order)
 
             # `Y` is a vector of length `order` that will be assigned the derivatives of `order` of the natural number in the corresponding row of `X`
             Y = sympy.zeros(order, 1)
 
             # It is possible that by choosing certain natural numbers, the system of equations will not be solvable, i.e. `X` is not invertible. This is unlikely but we check for invertibility of `X` for varying sets of natural numbers.
             invertible = False
             for t_ in range(1, max_t):
                 for i in range(order):
                     substitute = i + t_
-                    Y[i] = derivatives[order].subs(time_symbol, substitute)
+                    Y[i] = derivatives[order].subs(Config().input_time_symbol, substitute)
                     for j in range(order):
-                        X[i, j] = derivatives[j].subs(time_symbol, substitute)
+                        X[i, j] = derivatives[j].subs(Config().input_time_symbol, substitute)
 
-                if not _is_zero(sympy.simplify(sympy.det(X))):
+                if not _is_zero(sympy.det(X)):
                     invertible = True
                     break
 
             #
             #   If we failed to find an invertible `X`, it is very unlikely that the shape function obeys a linear homogeneous ODE of order `order` and we go on checking the next potential order.
             #
 
@@ -532,48 +518,48 @@
                 continue
 
 
             #
             #   calculate `derivative_factors`
             #
 
-            derivative_factors = sympy.simplify(X.inv() * Y)
+            derivative_factors = _custom_simplify_expr(X.inv() * Y)
 
 
             #
             #   fill in the obtained expressions for the derivative_factors and check whether they satisfy the definition of the shape
             #
 
             diff_rhs_lhs = 0
             logging.debug("\tchecking whether shape definition is satisfied...")
             for k in range(order):
                 diff_rhs_lhs -= derivative_factors[k] * derivatives[k]
             diff_rhs_lhs += derivatives[order]
 
-            if len(str(diff_rhs_lhs)) < Shape.EXPRESSION_SIMPLIFICATION_THRESHOLD and _is_zero(sympy.simplify(diff_rhs_lhs)):
+            if _is_zero(sympy.simplify(diff_rhs_lhs)):
                 found_ode = True
                 break
 
         if not found_ode:
             raise Exception("Shape does not satisfy any ODE of order <= " + str(max_order))
 
-        derivative_factors = [sympy.simplify(df) for df in derivative_factors]
+        derivative_factors = [_custom_simplify_expr(df) for df in derivative_factors]
 
 
         #
         #    calculate the initial values of the found ODE
         #
 
-        initial_values = {str(symbol) + derivative_order * '\'': x.subs(time_symbol, 0) for derivative_order, x in enumerate(derivatives[:-1])}
+        initial_values = {symbol + derivative_order * "'": x.subs(Config().input_time_symbol, 0) for derivative_order, x in enumerate(derivatives[:-1])}
 
-        return cls(symbol, order, initial_values, derivative_factors)
+        return cls(sympy.Symbol(symbol), order, initial_values, derivative_factors)
 
 
     @classmethod
-    def from_ode(cls, symbol: str, definition: str, initial_values: dict, all_variable_symbols=None, lower_bound=None, upper_bound=None, differential_order_symbol="__d", parameters=None, debug=False, **kwargs):
+    def from_ode(cls, symbol: str, definition: str, initial_values: dict, all_variable_symbols=None, lower_bound=None, upper_bound=None, parameters=None, debug=False, **kwargs) -> Shape:
         r"""
         Create a :python:`Shape` object given an ODE and initial values.
 
         Note that shapes are only aware of their own state variables: if an equation for :math:`x` depends on another state variable :math:`y` of another shape, then :math:`y` will be assumed to be a parameter and the term will appear in the inhomogeneous component of :math:`x`.
 
         :param symbol: The symbol (variable name) of the ODE.
         :param definition: The definition of the ODE.
@@ -592,28 +578,29 @@
         assert type(initial_values) is dict
 
         logging.info("\nProcessing differential-equation form shape " + str(symbol) + " with defining expression = \"" + str(definition) + "\"")
 
         if all_variable_symbols is None:
             all_variable_symbols = []
 
-        order = len(initial_values)
+        order: int = len(initial_values)
         all_variable_symbols_dict = {str(el): el for el in all_variable_symbols}
-        symbol = sympy.Symbol(symbol)
-        definition = sympy.parsing.sympy_parser.parse_expr(definition.replace("'", differential_order_symbol), global_dict=Shape._sympy_globals, local_dict=all_variable_symbols_dict)  # minimal global_dict to make no assumptions (e.g. "beta" could otherwise be recognised as a function instead of as a parameter symbol)
+        definition = sympy.parsing.sympy_parser.parse_expr(definition.replace("'", Config().differential_order_symbol), global_dict=Shape._sympy_globals, local_dict=all_variable_symbols_dict)  # minimal global_dict to make no assumptions (e.g. "beta" could otherwise be recognised as a function instead of as a parameter symbol)
         initial_values = {k: sympy.parsing.sympy_parser.parse_expr(v, global_dict=Shape._sympy_globals, local_dict=all_variable_symbols_dict) for k, v in initial_values.items()}
 
-        local_symbols = [sympy.Symbol(str(symbol) + differential_order_symbol * i) for i in range(order)]
+        local_symbols = [symbol + Config().differential_order_symbol * i for i in range(order)]
+        local_symbols_sympy = [sympy.Symbol(sym_name) for sym_name in local_symbols]
         if not symbol in all_variable_symbols:
-            all_variable_symbols.extend(local_symbols)
-        all_variable_symbols = [sympy.Symbol(str(sym_name).replace("'", differential_order_symbol)) for sym_name in all_variable_symbols]
-        derivative_factors, inhom_term, nonlin_term = Shape.split_lin_inhom_nonlin(definition, all_variable_symbols, parameters=parameters)
+            all_variable_symbols.extend(local_symbols_sympy)
+        all_variable_symbols = [str(sym_name).replace("'", Config().differential_order_symbol) for sym_name in all_variable_symbols]
+        all_variable_symbols_sympy = [sympy.Symbol(sym_name) for sym_name in all_variable_symbols]
+        derivative_factors, inhom_term, nonlin_term = Shape.split_lin_inhom_nonlin(definition, all_variable_symbols_sympy, parameters=parameters)
         local_symbols_idx = [all_variable_symbols.index(sym) for sym in local_symbols]
         local_derivative_factors = [derivative_factors[i] for i in local_symbols_idx]
-        nonlocal_derivative_terms = [derivative_factors[i] * all_variable_symbols[i] for i in range(len(all_variable_symbols)) if i not in local_symbols_idx]
+        nonlocal_derivative_terms = [derivative_factors[i] * all_variable_symbols_sympy[i] for i in range(len(all_variable_symbols)) if i not in local_symbols_idx]
         if nonlocal_derivative_terms:
             nonlin_term = nonlin_term + functools.reduce(lambda x, y: x + y, nonlocal_derivative_terms)
 
-        shape = cls(symbol, order, initial_values, local_derivative_factors, inhom_term, nonlin_term, lower_bound, upper_bound)
+        shape = cls(sympy.Symbol(symbol), order, initial_values, local_derivative_factors, inhom_term, nonlin_term, lower_bound, upper_bound)
         logging.info("\tReturning shape: " + str(shape))
 
         return shape
```

## odetoolbox/spike_generator.py

```diff
@@ -15,35 +15,38 @@
 # of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with NEST.  If not, see <http://www.gnu.org/licenses/>.
 #
 
+from typing import Mapping, List
+
 import io
 import math
 import numpy as np
 import random
-from typing import Mapping, List
+
+from .config import Config
 
 
 class SpikeGenerator():
 
     @classmethod
-    def spike_times_from_json(cls, stimuli, sim_time, derivative_symbol="__d") -> Mapping[str, List[float]]:
+    def spike_times_from_json(cls, stimuli, sim_time) -> Mapping[str, List[float]]:
         r"""
         Read or generate spike times according to a JSON specification.
 
         :return: spike_times: Each variable symbol is a key in the dictionary, and the list of spike times is the corresponding value. Symbol names use `derivative_symbol` to indicate differential order.
         """
         spike_times = {}
         for stimulus in stimuli:
             for sym in set(stimulus["variables"]):
                 assert type(sym) is str
-                sym = sym.replace("'", derivative_symbol)
+                sym = sym.replace("'", Config().differential_order_symbol)
                 if not sym in spike_times.keys():
                     spike_times[sym] = []
 
                 if stimulus["type"] == "poisson_generator":
                     spike_times[sym].extend(SpikeGenerator._generate_homogeneous_poisson_spikes(T=sim_time, rate=float(stimulus["rate"])))
                 elif stimulus["type"] == "regular":
                     spike_times[sym].extend(SpikeGenerator._generate_regular_spikes(T=sim_time, rate=float(stimulus["rate"])))
```

## odetoolbox/stiffness.py

```diff
@@ -30,16 +30,16 @@
 from .spike_generator import SpikeGenerator
 
 
 try:
     import pygsl.odeiv as odeiv
     PYGSL_AVAILABLE = True
 except ImportError as ie:
-    logging.warn("PyGSL is not available. The stiffness test will be skipped.")
-    logging.warn("Error when importing: " + str(ie))
+    logging.warning("PyGSL is not available. The stiffness test will be skipped.")
+    logging.warning("Error when importing: " + str(ie))
     PYGSL_AVAILABLE = False
 
 
 class StiffnessTester:
 
     def __init__(self, system_of_shapes, shapes, analytic_solver_dict=None, parameters=None, stimuli=None, random_seed=123, max_step_size=np.inf, integration_accuracy_abs=1E-6, integration_accuracy_rel=1E-6, sim_time=100., alias_spikes=False):
         r"""
@@ -107,15 +107,15 @@
         """
         assert PYGSL_AVAILABLE
 
         try:
             step_min_exp, step_average_exp, runtime_exp = self._evaluate_integrator(odeiv.step_rk4, raise_errors=raise_errors)
             step_min_imp, step_average_imp, runtime_imp = self._evaluate_integrator(odeiv.step_bsimp, raise_errors=raise_errors)
         except ParametersIncompleteException:
-            logging.warn("Stiffness test not possible because numerical values were not specified for all parameters.")
+            logging.warning("Stiffness test not possible because numerical values were not specified for all parameters.")
             return None
 
         # logging.info("runtime (imp:exp): %f:%f" % (runtime_imp, runtime_exp))
 
         return self._draw_decision(step_min_imp, step_min_exp, step_average_imp, step_average_exp)
```

## odetoolbox/system_of_shapes.py

```diff
@@ -23,19 +23,19 @@
 
 import logging
 import numpy as np
 import scipy
 import scipy.sparse
 import sympy
 import sympy.matrices
-import sys
 
+from .config import Config
 from .shapes import Shape
 from .singularity_detection import SingularityDetection
-from .sympy_printer import _is_zero
+from .sympy_helpers import _custom_simplify_expr, _is_zero
 
 
 def off_diagonal_is_zero(row: int, A) -> bool:
     for col in range(A.shape[1]):
         if col != row and not _is_zero(A[row, col]):
             return False
     return True
@@ -74,16 +74,16 @@
         for shape in self.shapes_:
             if str(shape.symbol) == sym:
                 return shape
         return None
 
     def get_initial_value(self, sym):
         for shape in self.shapes_:
-            if str(shape.symbol) == str(sym).replace("__d", "").replace("'", ""):
-                return shape.get_initial_value(sym.replace("__d", "'"))
+            if str(shape.symbol) == str(sym).replace(Config().differential_order_symbol, "").replace("'", ""):
+                return shape.get_initial_value(sym.replace(Config().differential_order_symbol, "'"))
 
         assert False, "Unknown symbol: " + str(sym)
 
 
     def get_dependency_edges(self):
         E = []
 
@@ -94,28 +94,28 @@
                 else:
                     if not _is_zero(sympy.diff(self.c_[j], sym1)):
                         E.append((sym2, sym1))
 
         return E
 
 
-    def get_lin_cc_symbols(self, E, differential_order_symbol="__d", parameters=None):
+    def get_lin_cc_symbols(self, E, parameters=None):
         r"""
         Retrieve the variable symbols of those shapes that are linear and constant coefficient. In the case of a higher-order shape, will return all the variable symbols with ``"__d"`` suffixes up to the order of the shape.
         """
         # get all symbols for all shapes as a list
         symbols = list(self.x_)
 
         node_is_lin = {}
         for shape in self.shapes_:
             if shape.is_lin_const_coeff_in(symbols, parameters=parameters):
                 _node_is_lin = True
             else:
                 _node_is_lin = False
-            all_shape_symbols = shape.get_state_variables(derivative_symbol=differential_order_symbol)
+            all_shape_symbols = shape.get_state_variables(derivative_symbol=Config().differential_order_symbol)
             for sym in all_shape_symbols:
                 node_is_lin[sym] = _node_is_lin
 
         return node_is_lin
 
 
     def propagate_lin_cc_judgements(self, node_is_lin, E):
@@ -168,35 +168,32 @@
         x_sub = self.x_[idx, :]
         A_sub = self.A_[idx, :][:, idx]
         b_sub = self.b_[idx, :]
 
         c_old = self.c_.copy()
         for _idx in idx:
             c_old[_idx] += self.A_[_idx, idx_compl].dot(self.x_[idx_compl, :])
-            if len(str(c_old[_idx])) > Shape.EXPRESSION_SIMPLIFICATION_THRESHOLD:
-                logging.warning("Skipping simplification of an expression that exceeds sympy simplification threshold")
-            else:
-                c_old[_idx] = sympy.simplify(c_old[_idx])
+            c_old[_idx] = _custom_simplify_expr(c_old[_idx])
 
         c_sub = c_old[idx, :]
 
         shapes_sub = [shape for shape in self.shapes_ if shape.symbol in symbols]
 
         return SystemOfShapes(x_sub, A_sub, b_sub, c_sub, shapes_sub)
 
 
-    def generate_propagator_solver(self, output_timestep_symbol: str = "__h"):
+    def generate_propagator_solver(self):
         r"""
         Generate the propagator matrix and symbolic expressions for propagator-based updates; return as JSON.
         """
         #
         #   generate the propagator matrix
         #
 
-        P = sympy.simplify(sympy.exp(self.A_ * sympy.Symbol(output_timestep_symbol)))
+        P = sympy.simplify(sympy.exp(self.A_ * sympy.Symbol(Config().output_timestep_symbol)))    # XXX: the default custom simplification expression does not work well with sympy 1.4 here. Consider replacing sympy.simplify() with _custom_simplify_expr() if sympy 1.4 support is dropped.
 
         if sympy.I in sympy.preorder_traversal(P):
             raise PropagatorGenerationException("The imaginary unit was found in the propagator matrix. This can happen if the dynamical system that was passed to ode-toolbox is unstable, i.e. one or more state variables will diverge to minus or positive infinity.")
 
         condition = SingularityDetection.find_singularities(P, self.A_)
         if condition:
             logging.warning("Under certain conditions, the propagator matrix is singular (contains infinities).")
@@ -229,53 +226,53 @@
                     if _is_zero(self.b_[col]):
                         # homogeneous ODE
                         update_expr_terms.append(sym_str + " * " + str(self.x_[col]))
                     else:
                         # inhomogeneous ODE
                         if _is_zero(self.A_[col, col]):
                             # of the form x' = const
-                            update_expr_terms.append(sym_str + " * " + str(self.x_[col]) + " + " + output_timestep_symbol + " * " + str(self.b_[col]))
+                            update_expr_terms.append(sym_str + " * " + str(self.x_[col]) + " + " + Config().output_timestep_symbol + " * " + str(self.b_[col]))
                         else:
                             particular_solution = -self.b_[col] / self.A_[col, col]
                             update_expr_terms.append(sym_str + " * (" + str(self.x_[col]) + " - (" + str(particular_solution) + "))" + " + (" + str(particular_solution) + ")")
 
             update_expr[str(self.x_[row])] = " + ".join(update_expr_terms)
             update_expr[str(self.x_[row])] = sympy.parsing.sympy_parser.parse_expr(update_expr[str(self.x_[row])], global_dict=Shape._sympy_globals)
             if not _is_zero(self.b_[row]):
                 # only simplify in case an inhomogeneous term is present
-                update_expr[str(self.x_[row])] = sympy.simplify(update_expr[str(self.x_[row])])
+                update_expr[str(self.x_[row])] = _custom_simplify_expr(update_expr[str(self.x_[row])])
 
         all_state_symbols = [str(sym) for sym in self.x_]
 
         initial_values = {sym: str(self.get_initial_value(sym)) for sym in all_state_symbols}
 
         solver_dict = {"propagators": P_expr,
                        "update_expressions": update_expr,
                        "state_variables": all_state_symbols,
                        "initial_values": initial_values}
 
         return solver_dict
 
 
-    def generate_numeric_solver(self, state_variables=None, simplify_expression="sympy.simplify(expr)"):
+    def generate_numeric_solver(self, state_variables=None):
         r"""
         Generate the symbolic expressions for numeric integration state updates; return as JSON.
         """
-        update_expr = self.reconstitute_expr(state_variables=state_variables, simplify_expression=simplify_expression)
+        update_expr = self.reconstitute_expr(state_variables=state_variables)
         all_state_symbols = [str(sym) for sym in self.x_]
         initial_values = {sym: str(self.get_initial_value(sym)) for sym in all_state_symbols}
 
         solver_dict = {"update_expressions": update_expr,
                        "state_variables": all_state_symbols,
                        "initial_values": initial_values}
 
         return solver_dict
 
 
-    def reconstitute_expr(self, state_variables=None, simplify_expression="sympy.simplify(expr)"):
+    def reconstitute_expr(self, state_variables=None):
         r"""
         Reconstitute a sympy expression from a system of shapes (which is internally encoded in the form :math:`\mathbf{x}' = \mathbf{Ax} + \mathbf{b} + \mathbf{c}`).
 
         Before returning, the expression is simplified using a custom series of steps, passed via the ``simplify_expression`` argument (see the ODE-toolbox documentation for more details).
         """
         if state_variables is None:
             state_variables = []
@@ -288,30 +285,19 @@
                 if str(self.A_[row, col]) in ["1", "1.", "1.0"]:
                     update_expr_terms.append(str(y))
                 else:
                     update_expr_terms.append(str(y) + " * (" + str(self.A_[row, col]) + ")")
             update_expr[str(x)] = " + ".join(update_expr_terms) + " + (" + str(self.b_[row]) + ") + (" + str(self.c_[row]) + ")"
             update_expr[str(x)] = sympy.parsing.sympy_parser.parse_expr(update_expr[str(x)], global_dict=Shape._sympy_globals)
 
-        # custom simplification steps (simplify() is not all that great)
-        try:
-            _simplify_expr = compile(simplify_expression, filename="<string>", mode="eval")
-            for name, expr in update_expr.items():
-                # skip simplification for long expressions
-                if len(str(expr)) > Shape.EXPRESSION_SIMPLIFICATION_THRESHOLD:
-                    logging.warning("Shape \"" + str(name) + "\" initialised with an expression that exceeds sympy simplification threshold")
-                    continue
-                update_expr[name] = eval(_simplify_expr)
-                collect_syms = [sym for sym in update_expr[name].free_symbols if not (sym in state_variables or str(sym) in state_variables)]
-                update_expr[name] = sympy.collect(update_expr[name], collect_syms)
-        except Exception as e:
-            logging.error("Exception occurred while applying expression simplification function: " + type(e).__name__)
-            logging.error(str(e))
-            logging.error("Check that the parameter ``simplify_expression`` is properly formatted.")
-            sys.exit(1)
+        # custom expression simplification
+        for name, expr in update_expr.items():
+            update_expr[name] = _custom_simplify_expr(expr)
+            collect_syms = [sym for sym in update_expr[name].free_symbols if not (sym in state_variables or str(sym) in state_variables)]
+            update_expr[name] = sympy.collect(update_expr[name], collect_syms)
 
         return update_expr
 
 
     def shape_order_from_system_matrix(self, idx: int) -> int:
         r"""Determine shape differential order from system matrix of symbol ``self.x_[idx]``"""
         N = self.A_.shape[0]
@@ -366,20 +352,20 @@
         A = sympy.zeros(N, N)
         b = sympy.zeros(N, 1)
         c = sympy.zeros(N, 1)
 
         i = 0
         for shape in shapes:
             for j in range(shape.order):
-                x[i] = shape.get_state_variables(derivative_symbol="__d")[j]
+                x[i] = shape.get_state_variables(derivative_symbol=Config().differential_order_symbol)[j]
                 i += 1
 
         i = 0
         for shape in shapes:
-            highest_diff_sym_idx = [k for k, el in enumerate(x) if el == sympy.Symbol(str(shape.symbol) + "__d" * (shape.order - 1))][0]
+            highest_diff_sym_idx = [k for k, el in enumerate(x) if el == sympy.Symbol(str(shape.symbol) + Config().differential_order_symbol * (shape.order - 1))][0]
             shape_expr = shape.reconstitute_expr()
 
             #
             #   grab the defining expression and separate into linear and nonlinear part
             #
 
             lin_factors, inhom_term, nonlin_term = Shape.split_lin_inhom_nonlin(shape_expr, x, parameters=parameters)
```

## Comparing `odetoolbox/sympy_printer.py` & `odetoolbox/sympy_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 # of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with NEST.  If not, see <http://www.gnu.org/licenses/>.
 #
 
+import logging
 import sympy
-from sympy.printing import StrPrinter
+import sys
+
+from .config import Config
 
 
 def _is_zero(x):
     r"""
     Check if a sympy expression is equal to zero.
 
     In the ideal case, we would like to use sympy.simplify() to do simplification of an expression before comparing it to zero. However, for expressions of moderate size (e.g. a few dozen terms involving exp() functions), it becomes unbearably slow. We therefore use this internal function, so that the simplification function can be easily switched over.
@@ -48,15 +51,36 @@
         return isinstance(var, sympy.Basic)
     except:  # noqa
         pass
 
     raise Exception("Unsupported sympy version used")
 
 
-class SympyPrinter(StrPrinter):
+def _custom_simplify_expr(expr: str):
+    """Custom expression simplification"""
+    if isinstance(expr, sympy.matrices.MatrixBase):
+        return expr.applyfunc(_custom_simplify_expr)
+
+    try:
+        # skip simplification for long expressions
+        if len(str(expr)) > Config().expression_simplification_threshold:
+            logging.warning("Length of expression \"" + str(expr) + "\" exceeds sympy simplification threshold")
+
+        _simplify_expr = compile(Config().simplify_expression, filename="<string>", mode="eval")
+        expr_simplified = eval(_simplify_expr)
+
+        return expr_simplified
+    except Exception as e:
+        print("Exception occurred while applying expression simplification function: " + type(e).__name__)
+        print(str(e))
+        print("Check that the parameter ``simplify_expression`` is properly formatted.")
+        sys.exit(1)
+
+
+class SympyPrinter(sympy.printing.StrPrinter):
 
     def _print_Exp1(self, expr):
         return 'e'
 
     def _print_Function(self, expr):
         """
         Overrides base class method to print min() and max() functions in lowercase.
```

## Comparing `odetoolbox-2.5.data/scripts/ode_analyzer.py` & `odetoolbox-2.5.1.data/scripts/ode_analyzer.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     argparser = argparse.ArgumentParser(description="""ode-toolbox -- https://github.com/nest/ode-toolbox""", formatter_class=argparse.RawDescriptionHelpFormatter)
 
     argparser.add_argument("infile", metavar='PATH', type=str, help="JSON input file path")
     argparser.add_argument("--disable-stiffness-check", action="store_true", help="If provided, disable stiffness check")
     argparser.add_argument("--disable-analytic-solver", action="store_true", help="If provided, disable generation of propagators")
     argparser.add_argument("--preserve-expressions", action="store", nargs="*", default=False, help="Set to True, or a list of strings corresponding to individual variable names, to disable internal rewriting of expressions, and return same output as input expression where possible. Can only apply to variables specified as first-order differential equations.")
-    argparser.add_argument("--simplify-expression", action="store", default="sympy.simplify(expr)", help="For all expressions ``expr`` that are rewritten internally: the contents of this parameter string are evaluated with ``eval()`` in Python to obtain the final output expression. Override for custom expression simplification steps. Example: ``\"sympy.logcombine(sympy.powsimp(sympy.expand(expr)))\"``.")
     argparser.add_argument("--log-level", action="store", default="WARN", help="Sets the logging threshold. Logging messages which are less severe than ``log_level`` will be ignored. Log levels can be provided as an integer or string, for example \"INFO\" (more messages) or \"WARN\" (fewer messages). For a list of valid logging levels, see https://docs.python.org/3/library/logging.html#logging-levels")
     parsed_args = argparser.parse_args()
 
     if isinstance(parsed_args.preserve_expressions, Iterable) and len(parsed_args.preserve_expressions) == 0:
         parsed_args.preserve_expressions = True
 
     _init_logging(log_level=parsed_args.log_level)
@@ -65,15 +64,14 @@
             sys.exit(1)
 
     try:
         result = odetoolbox.analysis(indict,
                                      disable_stiffness_check=parsed_args.disable_stiffness_check,
                                      disable_analytic_solver=parsed_args.disable_analytic_solver,
                                      preserve_expressions=parsed_args.preserve_expressions,
-                                     simplify_expression=parsed_args.simplify_expression,
                                      log_level=parsed_args.log_level)
     except MalformedInputException as e:
         logging.error("The input JSON file could not be parsed; error: " + e.message)
         sys.exit(1)
 
     basename = os.path.basename(parsed_args.infile.rsplit(".", 1)[0])
     outfname = "%s_result.json" % basename
```

## Comparing `odetoolbox-2.5.dist-info/LICENSE.md` & `odetoolbox-2.5.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `odetoolbox-2.5.dist-info/METADATA` & `odetoolbox-2.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odetoolbox
-Version: 2.5
+Version: 2.5.1
 Summary: ODE-toolbox: Automatic selection and generation of integration schemes for systems of ordinary differential equations
 Home-page: https://github.com/nest/ode-toolbox
 Author: The NEST Initiative
 License: GNU General Public License v2 (GPLv2)
 Keywords: computational neuroscience model ordinary differential equation ode dynamical dynamic simulation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

