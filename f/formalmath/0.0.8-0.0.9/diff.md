# Comparing `tmp/formalmath-0.0.8.tar.gz` & `tmp/formalmath-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formalmath-0.0.8.tar", last modified: Thu Jun  8 19:45:07 2023, max compression
+gzip compressed data, was "formalmath-0.0.9.tar", last modified: Fri Jun  9 02:05:59 2023, max compression
```

## Comparing `formalmath-0.0.8.tar` & `formalmath-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.181896 formalmath-0.0.8/
--rw-rw-rw-   0        0        0     3278 2023-06-08 19:45:07.181896 formalmath-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2832 2023-06-08 19:42:24.000000 formalmath-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.179896 formalmath-0.0.8/formalmath/
--rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.8/formalmath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.181896 formalmath-0.0.8/formalmath/setmm/
--rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.8/formalmath/setmm/__init__.py
--rw-rw-rw-   0        0        0    18579 2023-06-08 19:34:27.000000 formalmath-0.0.8/formalmath/setmm/basic_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.180895 formalmath-0.0.8/formalmath.egg-info/
--rw-rw-rw-   0        0        0     3278 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 19:45:07.181896 formalmath-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-06-08 19:44:26.000000 formalmath-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:05:59.054902 formalmath-0.0.9/
+-rw-rw-rw-   0        0        0     4497 2023-06-09 02:05:59.053902 formalmath-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4051 2023-06-09 02:05:15.000000 formalmath-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 02:05:59.052902 formalmath-0.0.9/formalmath/
+-rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.9/formalmath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:05:59.053902 formalmath-0.0.9/formalmath/setmm/
+-rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.9/formalmath/setmm/__init__.py
+-rw-rw-rw-   0        0        0    22015 2023-06-09 01:53:53.000000 formalmath-0.0.9/formalmath/setmm/basic_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-09 02:05:59.053902 formalmath-0.0.9/formalmath.egg-info/
+-rw-rw-rw-   0        0        0     4497 2023-06-09 02:05:59.000000 formalmath-0.0.9/formalmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-09 02:05:59.000000 formalmath-0.0.9/formalmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 02:05:59.000000 formalmath-0.0.9/formalmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-09 02:05:59.000000 formalmath-0.0.9/formalmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 02:05:59.054902 formalmath-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-09 02:05:29.000000 formalmath-0.0.9/setup.py
```

### Comparing `formalmath-0.0.8/README.md` & `formalmath-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 # formalmath
 
 A formal mathematics package.
 
+## Install
+
+```
+pip install formalmath
+```
+
 ## setmm
 
 A port for [metamath](https://us.metamath.org) and `set.mm`. The language `metamath` is a math proof verifying language. And, `set.mm` is its main database of theorems, based on the classical ZFC axiom system.
 
-`MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
+`MObject` is the basic type Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
+
+ `Constant` is the type of constants, corresponding to $c statements in metamath.
+
+`Variable` is the type of variables, corresponding to $v statements in metamath.
 
- `Constant` is the class of constants, corresponding to $c statements in metamath.
+`Formula` is the base type of formulas, corresponding to wff in metamath and set.mm.
 
-`Variable` is the class of variables, corresponding to $v statements in metamath.
+`FormulaConstant` are Constant objects that are also Formulas.
 
-`Formula` is the base class of formulas, corresponding to wff in metamath and set.mm.
+`FormulaVariable` are Variable objects that are also Formulas.
 
-`FormulaVariable` is the class of formula with only one symbol.
+`ClassType` is the base type of classes, corresponding to class in metamath and set.mm.
 
-`FormulaTemplate` is the class of templates that generate new formula out of old formulas and other symbols.
+`ClassConstant` are Constant objects that are also `ClassType` objects.
+
+`ClassVariable` are Variable objects that are also `ClassType` objects.
+
+`Template` are base type of templates. A template can generate new formula or class out of old.
+
+`FormulaTemplate` denote templates that generate new formula out of old formulas and other symbols.
+
+`ClassTemplate` denote templates that generate new `ClassType` objects out of old `ClassType` objects and other symbols.
+
+`SetVariable` denote `setvar` notation in metamath and set.mm.
 
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath.setmm import *
@@ -72,9 +92,25 @@
 # Template:  (  (  (  y  ->  z  )  ->  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ) 
 #  ->  (  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ->  w  )  )
 # Types:
 # y : Formula
 # z : Formula
 # x : Formula
 # w : Formula
+one = ClassConstant("1")
+two = ClassConstant("2")
+three = ClassConstant("3")
+equal = Constant("=")
+plus = Constant("+")
+temp_plus = ClassTemplate({"var_types":{"a":ClassType,"b":ClassType},"template":["a",plus,"b"]})
+temp_eq = FormulaTemplate({"var_types":{"u":ClassType,"v":ClassType},"template":["u",equal,"v"]})
+temp_new = temp_eq.generate_template({"u":temp_plus,"v":"c"})
+print(temp_new)
+# Template:  a  +  b  =  c
+# Types:
+# a : ClassType
+# b : ClassType
+# c : ClassType
+eq1p2e3 = temp_new.generate({"a":one,"b":two,"c":three})
+print(eq1p2e3) # Formula("1 + 2 = 3")
 ```
```

### Comparing `formalmath-0.0.8/formalmath/setmm/basic_classes.py` & `formalmath-0.0.9/formalmath/setmm/basic_classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 '''
 Python port for a slightly extended version of the formal language metamath (us.metamath.org) and the theorem database set.mm written by metamath. This system includes over 40000 theorems in the classic ZFC axiom system.
 
 The basic classes will be defined in this file. That includes:
-0. MObject. The base class for all classes.
-1. Constant. That correspond to $c statement in metamath.
-2. Variable. That correspond to $v statement in metamath.
-3. FormulaTemplate. That correspond to $a statements starting with wff symbol. Basically, it generates new formula from old. But the template's symbol list can also have Constant, ClassVariable, ClassType, SetVariable, etc.
-4. Formula. That correspond to wff in metamath and set.mm. It is not a part of the basic metamath language. But it is defined in set.mm to denote well formed formula. There is always new ways to form a wff, when a new term is introduced. But all of them correspond to a conbination of old terms.
-5. ClassType. That correspond to class in metamath and set.mm.
-6. ClassVariable. That correspond to class denoted by a single symbol in metamath and set.mm.
+1. MObject. The base class for all classes.
+2. Constant. That correspond to $c statement in metamath.
+2.1. FormulaConstant. Constants that are also Formula objects.
+2.2. ClassConstant. Constants that are also ClassType objects.
+3. Variable. That correspond to $v statement in metamath.
+4. Template. That correspond to $a and $p statements starting with wff symbol or class symbol. Basically, it generates new formula and class from old. But the template's symbol list can also have Constant, ClassType, SetVariable, etc.
+4.1. FormulaTemplate. Templates that generates well formed formulas.
+4.2. ClassTemplate. Templates that generates classes.
+5. Formula. That correspond to wff in metamath and set.mm. It is not a part of the basic metamath language. But it is defined in set.mm to denote well formed formula. There is always new ways to form a wff, when a new term is introduced. But all of them correspond to a conbination of old terms.
+5.1. FormulaVariable. That correspond to wff denoted by a single symbol in metamath and set.mm. 
+6. ClassType. That correspond to class in metamath and set.mm.
+6.1. ClassVariable. That correspond to class denoted by a single symbol in metamath and set.mm.
 7. SetVariable. That correspond to setvar in metamath and set.mm.
-8. Axiom. That correspond to $a statements that are axioms.
-9. Definition. That correspond to $a statements that are definitions.
+8. Proposition. It's a basic type for all axioms, definitions, theorems and conjectures.
+9. Axiom. That correspond to $a statements that are axioms.
+10. Definition. That correspond to $a statements that are definitions.
+11. Theorem. That correspond to $p statements. Require a correct proof ( $= (proof) $. part ).
+12. Conjecture. That are $p statements without proof.
 
 Inherit relation:
-MObject ----- Constant
+
+MObject ----- Constant ----- FormulaConstant (also inherit from Formula)
+          |              |-- ClassConstant (also inherit from ClassType)
           |
-          |-- Variable -- SetVariable
+          |-- Variable ----- SetVariable
+          |              |-- FormulaVariable (also inherit from Formula)
+          |              |-- ClassVariable (also inherit from ClassType)
           |         
-          |-- Formula -- FormulaVariable (also inherit Variable)
+          |-- Formula
           |
-          |-- FormulaTemplate
+          |-- ClassType
           |
-          |-- ClassType -- ClassVariable (also inherit Variable)
+          |-- Template ----- FormulaTemplate
+                         |-- ClassTemplate
 
 Some basic constants will be defined here too, such as left and right parenthesis, well-formed formula symbol and turnstile.
 '''
 
 class MObject:
     '''
     Base class for all metamath classes.
@@ -61,15 +74,16 @@
         if metamath_code:
             # ensure the uniqueness of metamath_code
             self._check_unique_metamath_code(metamath_code)
             # define the metamath_code of an MObject
             self.metamath_code = metamath_code
 
         # add the new MObject into dicts
-        MObject.MObject_labels[label] = self
+        if label:
+            MObject.MObject_labels[label] = self
         if latex_code:
             MObject.MObject_latex_codes[latex_code] = self
         if metamath_code:
             MObject.MObject_metamath_codes[metamath_code] = self
     
     def _check_unique_label(self, label):
         '''
@@ -197,15 +211,26 @@
     
     def __str__(self):
         '''
         print Formula. will override the __str__ method in MObject.
         '''
         labelstr = ' '.join([f"{s.label}" for s in self.list_of_symbols])
         return f"Formula(\"{labelstr}\")"
+
+class FormulaConstant(Constant, Formula):
+    '''
+    Constants that are also well formed formulas.
+    '''
+    def __init__(self, label=None, latex_code=None, metamath_code=None, list_of_symbols=None):
+        super().__init__(label, latex_code, metamath_code)
+        self.list_of_symbols=[self]
     
+    def __str__(self):
+        return f"FormulaConstant(\"{self.label}\")"
+
 class FormulaVariable(Variable, Formula):
     '''
     $f statement of form $f wff varname $. It means that varname represents a well formed formula.
     This class is the special kind of Formula consisting of only one variable.
     '''
     def __init__(self, label=None, latex_code=None, metamath_code=None):
         super().__init__(label, latex_code, metamath_code)
@@ -244,72 +269,82 @@
                 raise TypeError(f"{symbol}: not in supported type. We support Constant, Formula, ClassType and SetVariable for symbols in list_of_symbols.")
     
     def __str__(self):
         '''
         print ClaaType. will override the __str__ method in MObject.
         '''
         labelstr = ' '.join([f"{s.label}" for s in self.list_of_symbols])
-        return f"Formula(\"{labelstr}\")"
+        return f"Class(\"{labelstr}\")"
+
+class ClassConstant(Constant, ClassType):
+    '''
+    Constants that are also ClassType objects.
+    '''
+    def __init__(self, label=None, latex_code=None, metamath_code=None):
+        super().__init__(label, latex_code, metamath_code)
+        self.list_of_symbols=[self]
+
+    def __str__(self):
+        return f"ClassConstant(\"{self.label}\")"
 
 class ClassVariable(Variable, ClassType):
     '''
     $f statement of form $f class varname $. It means that varname represents a class.
     '''
     def __init__(self, label=None, latex_code=None, metamath_code=None):
         super().__init__(label, latex_code, metamath_code)
         self.list_of_symbols = [self]
     
     def __str__(self):
-        return f"ClassVariable(\"{self.label}\")"
+        return f"Class(\"{self.label}\")"
 
 class SetVariable(Variable):
     '''
     $f statement of form $f setvar varname $. It means that varname represents a set variable.
     '''
     def __init__(self, label=None, latex_code=None, metamath_code=None):
         super().__init__(label, latex_code, metamath_code)
     
     def __str__(self):
         return f"SetVariable(\"{self.label}\")"
 
-class FormulaTemplate(MObject):
+class Template(MObject):
     '''
-    $a statements that generates new Formula from old by substitution.
+    $a statements that generates new Formula or ClassType from old by substitution.
     '''
     def __init__(self, template=None, label=None, latex_code=None, metamath_code=None):
         '''
         template: a dictionary that has keys "var_types" and "template"
         example: {"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]}
         this example means in the Template of Formula "( x -> y )", x, y should be replaced with Formulas.
         '''
         super().__init__(label, latex_code, metamath_code)
         # check that the template has the right format.
         self._check_template(template)            
         setattr(self, "template", template)
         
-    def generate(self, vars, mylabel=None, mycode=None, mymmcode=None):
+    def _generate(self, vars):
         '''
-        use the template to define a generator of new Formula from old
+        use the template to define a generator of new Formula or ClassType from old
         '''
         mylist = []
         for symbol in self.template["template"]:
             if isinstance(symbol,str):
                 if self.template["var_types"][symbol] in [Formula,ClassType]:
-                    if len(vars[symbol].list_of_symbols) > 1:
-                        mylist = mylist + vars[symbol].list_of_symbols
-                    else:
-                        mylist.append(vars[symbol])
+                    # if len(vars[symbol].list_of_symbols) > 1:
+                    mylist = mylist + vars[symbol].list_of_symbols
+                    # else:
+                    # mylist.append(vars[symbol])
                 else:
                     mylist.append(vars[symbol])
             else:
                 mylist.append(symbol)
-        newFormula = Formula(mylabel,mycode,mymmcode,mylist)
-        return newFormula
+        return mylist
     
-    def generate_template(self, vars, mylabel=None, mycode=None, mymmcode=None):
+    def _generate_template(self, vars):
         '''
         use the template to define a generator of new FormulaTemplate from old 
         '''
         new_var_types = {}
         new_template = []
         var_types = self.template["var_types"]
         temp = self.template["template"]
@@ -327,15 +362,15 @@
         for item in vars.keys():
             if isinstance(vars[item], str):
                 if vars[item] not in new_var_types.keys():
                     new_var_types[vars[item]] = var_types[item]
                 else:
                     if new_var_types[vars[item]] != var_types[item]:
                         raise ValueError(f"Conflict types: {new_var_types[vars[item]]} and {var_types[item]}")
-            elif isinstance(vars[item], FormulaTemplate):
+            elif isinstance(vars[item], Template):
                 for symbol in vars[item].template["var_types"].keys():
                     if symbol not in new_var_types.keys():
                         new_var_types[symbol] = vars[item].template["var_types"][symbol]
                     else:
                         if new_var_types[symbol] != vars[item].template["var_types"][symbol]:
                             raise ValueError(f"Conflict types: {new_var_types[symbol]} and {vars[item].template['var_types'][symbol]}")
             else:
@@ -344,22 +379,22 @@
         for symbol in temp:
             if isinstance(symbol, str):
                 if isinstance(vars[symbol],str):
                     new_template.append(vars[symbol])
                 else:
                     if symbol not in vars.keys():
                         raise ValueError(f"Undefined symbol : {symbol}")
-                    if not isinstance(vars[symbol],FormulaTemplate):
+                    if not isinstance(vars[symbol],Template):
                         raise ValueError(f"Unsupported type : {vars[symbol]}")
                     new_template = new_template + vars[symbol].template["template"]
             else:
                 new_template.append(symbol)
         
-        new_formula_temp = FormulaTemplate({"var_types":new_var_types,"template":new_template},mylabel,mycode,mymmcode)
-        return new_formula_temp
+        new_temp = {"var_types":new_var_types,"template":new_template}
+        return new_temp
 
     def _check_template(self, template):
         '''
         check that the template has the right format.
         '''
         if not isinstance(template["template"], list):
             raise ValueError(f"Template is not a list.")
@@ -371,32 +406,58 @@
                 if not isinstance(symbol,str):
                     raise ValueError("Template format error.")
                 if symbol not in vars:
                     raise ValueError(f"Found undefined symbol in template: {symbol}")
         
         for item in vars:
             # ensure that the type assignings in template["var_types"] are supported (Formula, SetVariable, ClassVariable)
-            if template["var_types"][item] not in [Formula, SetVariable, ClassVariable]:
+            if template["var_types"][item] not in [Formula, SetVariable, ClassType]:
                 raise ValueError(f"Found unsupported type in template: {item}:{template['var_types'][item]}")
         
     def __str__(self):
         temp_str = ""
         for symbol in self.template["template"]:
             if isinstance(symbol, str):
                 temp_str += f" {symbol} "
             else:
                 temp_str += f" {symbol.label} "
         vartype_str = ""
         for v in self.template["var_types"].keys():
             vartype_str += f"{v} : {self.template['var_types'][v].__name__}\n"
         return f"Template: {temp_str}\nTypes:\n{vartype_str}"
 
+class FormulaTemplate(Template):
+    '''
+    $a statements that generates new Formula from old by substitution.
+    '''
+    def __init__(self, template=None, label=None, latex_code=None, metamath_code=None):
+        super().__init__(template, label, latex_code, metamath_code)
+    
+    def generate(self, vars, label=None, latex_code=None, metamath_code=None):
+        list_of_symbols = self._generate(vars)
+        return Formula(label, latex_code, metamath_code, list_of_symbols)
+    
+    def generate_template(self, vars, mylabel=None, mycode=None, mymmcode=None):
+        temp = self._generate_template(vars)
+        return FormulaTemplate(temp,mylabel,mycode,mymmcode)
 
-
-
+class ClassTemplate(Template):
+    '''
+    $a statements that generates new ClassType from old by substitution.
+    '''
+    def __init__(self, template=None, label=None, latex_code=None, metamath_code=None):
+        super().__init__(template, label, latex_code, metamath_code)
+    
+    def generate(self, vars, label=None, latex_code=None, metamath_code=None):
+        list_of_symbols = self._generate(vars)
+        return ClassType(label, latex_code, metamath_code, list_of_symbols)
+    
+    def generate_template(self, vars, mylabel=None, mycode=None, mymmcode=None):
+        temp = self._generate_template(vars)
+        return ClassTemplate(temp,mylabel,mycode,mymmcode)
 
 if __name__=='__main__':
     lp = Constant("(")
     rp = Constant(")")
     ra = Constant("->")
     phi = FormulaVariable("phi")
     psi = FormulaVariable("psi")
@@ -428,8 +489,24 @@
     print(wi3)
     # Template:  (  (  (  y  ->  z  )  ->  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ) 
     #  ->  (  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ->  w  )  )
     # Types:
     # y : Formula
     # z : Formula
     # x : Formula
-    # w : Formula
+    # w : Formula
+    one = ClassConstant("1")
+    two = ClassConstant("2")
+    three = ClassConstant("3")
+    equal = Constant("=")
+    plus = Constant("+")
+    temp_plus = ClassTemplate({"var_types":{"a":ClassType,"b":ClassType},"template":["a",plus,"b"]})
+    temp_eq = FormulaTemplate({"var_types":{"u":ClassType,"v":ClassType},"template":["u",equal,"v"]})
+    temp_new = temp_eq.generate_template({"u":temp_plus,"v":"c"})
+    print(temp_new)
+    # Template:  a  +  b  =  c
+    # Types:
+    # a : ClassType
+    # b : ClassType
+    # c : ClassType
+    eq1p2e3 = temp_new.generate({"a":one,"b":two,"c":three})
+    print(eq1p2e3) # Formula("1 + 2 = 3")
```

### Comparing `formalmath-0.0.8/setup.py` & `formalmath-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="formalmath",  # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="a python port of formal mathematics proof verifier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/formalmath.git",
     packages=setuptools.find_packages(),
```

