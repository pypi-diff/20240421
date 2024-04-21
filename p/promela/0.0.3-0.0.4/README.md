# Comparing `tmp/promela-0.0.3.tar.gz` & `tmp/promela-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promela-0.0.3.tar", last modified: Mon Sep 14 13:32:42 2020, max compression
+gzip compressed data, was "promela-0.0.4.tar", last modified: Sun Apr 21 14:25:14 2024, max compression
```

## Comparing `promela-0.0.3.tar` & `promela-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2020-09-14 13:32:42.367310 promela-0.0.3/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1586 2020-09-14 13:29:41.000000 promela-0.0.3/LICENSE
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)       68 2020-09-14 13:29:11.000000 promela-0.0.3/MANIFEST.in
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1956 2020-09-14 13:32:42.367310 promela-0.0.3/PKG-INFO
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      881 2020-09-14 13:29:41.000000 promela-0.0.3/README.md
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     3756 2020-09-14 13:29:11.000000 promela-0.0.3/doc.md
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2020-09-14 13:32:42.367310 promela-0.0.3/promela/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      148 2020-09-14 13:29:11.000000 promela-0.0.3/promela/__init__.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)       58 2020-09-14 13:32:39.000000 promela-0.0.3/promela/_version.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)    29654 2020-09-14 13:29:41.000000 promela-0.0.3/promela/ast.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     5380 2020-09-14 13:29:11.000000 promela-0.0.3/promela/lex.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)   103007 2020-09-14 13:32:42.000000 promela-0.0.3/promela/promela_parsetab.py
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)    24870 2020-09-14 13:29:11.000000 promela-0.0.3/promela/yacc.py
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2020-09-14 13:32:42.367310 promela-0.0.3/promela.egg-info/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1956 2020-09-14 13:32:42.000000 promela-0.0.3/promela.egg-info/PKG-INFO
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)      332 2020-09-14 13:32:42.000000 promela-0.0.3/promela.egg-info/SOURCES.txt
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)        1 2020-09-14 13:32:42.000000 promela-0.0.3/promela.egg-info/dependency_links.txt
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)       43 2020-09-14 13:32:42.000000 promela-0.0.3/promela.egg-info/requires.txt
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)        8 2020-09-14 13:32:42.000000 promela-0.0.3/promela.egg-info/top_level.txt
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)       38 2020-09-14 13:32:42.367310 promela-0.0.3/setup.cfg
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2118 2020-09-14 13:29:41.000000 promela-0.0.3/setup.py
-drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2020-09-14 13:32:42.367310 promela-0.0.3/tests/
--rw-r--r--   0 ioannis   (1000) ioannis   (1000)    15464 2020-09-14 13:29:11.000000 promela-0.0.3/tests/yacc_test.py
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-21 14:25:14.115446 promela-0.0.4/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1586 2024-04-21 14:18:48.000000 promela-0.0.4/LICENSE
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)       68 2024-04-21 14:18:48.000000 promela-0.0.4/MANIFEST.in
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1659 2024-04-21 14:25:14.115446 promela-0.0.4/PKG-INFO
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      730 2024-04-21 14:18:48.000000 promela-0.0.4/README.md
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     3772 2024-04-21 14:18:48.000000 promela-0.0.4/doc.md
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-21 14:25:14.115446 promela-0.0.4/promela/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      181 2024-04-21 14:18:48.000000 promela-0.0.4/promela/__init__.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)       58 2024-04-21 14:25:12.000000 promela-0.0.4/promela/_version.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)    29993 2024-04-21 14:18:48.000000 promela-0.0.4/promela/ast.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     5937 2024-04-21 14:18:48.000000 promela-0.0.4/promela/lex.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)   103007 2024-04-21 14:25:13.000000 promela-0.0.4/promela/promela_parsetab.py
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)    25098 2024-04-21 14:18:48.000000 promela-0.0.4/promela/yacc.py
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-21 14:25:14.115446 promela-0.0.4/promela.egg-info/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     1659 2024-04-21 14:25:14.000000 promela-0.0.4/promela.egg-info/PKG-INFO
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)      332 2024-04-21 14:25:14.000000 promela-0.0.4/promela.egg-info/SOURCES.txt
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)        1 2024-04-21 14:25:14.000000 promela-0.0.4/promela.egg-info/dependency_links.txt
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)       30 2024-04-21 14:25:14.000000 promela-0.0.4/promela.egg-info/requires.txt
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)        8 2024-04-21 14:25:14.000000 promela-0.0.4/promela.egg-info/top_level.txt
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)       38 2024-04-21 14:25:14.115446 promela-0.0.4/setup.cfg
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)     2485 2024-04-21 14:18:48.000000 promela-0.0.4/setup.py
+drwxr-xr-x   0 ioannis   (1000) ioannis   (1000)        0 2024-04-21 14:25:14.115446 promela-0.0.4/tests/
+-rw-r--r--   0 ioannis   (1000) ioannis   (1000)    15433 2024-04-21 14:18:48.000000 promela-0.0.4/tests/yacc_test.py
```

### Comparing `promela-0.0.3/LICENSE` & `promela-0.0.4/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (c) 2014-2020 by California Institute of Technology
-Copyright (c) 2014-2020 by Ioannis Filippidis
+Copyright (c) 2014-2022 by California Institute of Technology
+Copyright (c) 2014-2022 by Ioannis Filippidis
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `promela-0.0.3/PKG-INFO` & `promela-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: promela
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parser and abstract syntax tree for the Promela modeling language.
 Home-page: https://github.com/johnyf/promela
 Author: Ioannis Filippidis
 Author-email: jfilippidis@gmail.com
 License: BSD
-Description: [![Build Status][build_img]][travis]
-        [![Coverage Status][coverage]][coveralls]
-        
-        
-        About
-        =====
-        
-        A parser for the [Promela modeling language](https://en.wikipedia.org/wiki/Promela).
-        [PLY](https://pypi.python.org/pypi/ply/3.4) (Python `lex`-`yacc`) is used to generate the parser.
-        Classes for a Promela abstract tree are included and used for representing the result of parsing.
-        A short tutorial can be found in the file [`doc.md`](
-            https://github.com/johnyf/promela/blob/master/doc.md).
-        To install:
-        
-        ```
-        pip install promela
-        ```
-        
-        
-        License
-        =======
-        [BSD-3](http://opensource.org/licenses/BSD-3-Clause), see `LICENSE` file.
-        
-        
-        [build_img]: https://travis-ci.org/johnyf/promela.svg?branch=master
-        [travis]: https://travis-ci.org/johnyf/promela
-        [coverage]: https://coveralls.io/repos/johnyf/promela/badge.svg?branch=master
-        [coveralls]: https://coveralls.io/r/johnyf/promela?branch=master
-        
+Project-URL: Bug Tracker, https://github.com/johnyf/promela/issues
+Project-URL: Documentation, https://github.com/johnyf/promela/blob/main/doc.md
 Keywords: promela,parser,syntax tree,ply,lex,yacc
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: networkx>=2.0
+Requires-Dist: ply<=3.10,>=3.4
+
+[![Build Status][build_img]][ci]
+
+
+About
+=====
+
+A parser for the [Promela modeling language](https://en.wikipedia.org/wiki/Promela).
+[PLY](https://pypi.org/project/ply/3.4/) (Python `lex`-`yacc`) is used to
+generate the parser. Classes for a Promela abstract tree are included and used
+for representing the result of parsing.
+
+A short tutorial can be found in the file [`doc.md`](
+    https://github.com/johnyf/promela/blob/main/doc.md).
+To install:
+
+```
+pip install promela
+```
+
+
+License
+=======
+
+[3-clause BSD](https://opensource.org/licenses/BSD-3-Clause),
+see the file `LICENSE`.
+
+
+[build_img]: https://github.com/johnyf/promela/actions/workflows/main.yml/badge.svg?branch=main
+[ci]: https://github.com/johnyf/promela/actions
```

### Comparing `promela-0.0.3/doc.md` & `promela-0.0.4/doc.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-This package provides a lexer, parser, and abstract syntax tree (AST) for the [Promela](http://en.wikipedia.org/wiki/Promela) modeling language.
-The lexer and parser are generated using [PLY](https://pypi.python.org/pypi/ply/3.4) (Python `lex`-`yacc`).
-The [grammar](http://spinroot.com/spin/Man/grammar.html) is based on that used in the [SPIN](http://spinroot.com/spin/whatispin.html) model checker (in the files `spin.y` and `spinlex.c` of SPIN's source distribution), with modifications where needed.
+This package provides a lexer, parser, and abstract syntax tree (AST) for the
+[Promela](https://en.wikipedia.org/wiki/Promela) modeling language.
+The lexer and parser are generated using [PLY](
+    https://pypi.org/project/ply/3.4/)
+(Python `lex`-`yacc`).
+The [grammar](https://spinroot.com/spin/Man/grammar.html) is based on that used
+in the [SPIN](https://spinroot.com/spin/whatispin.html) model checker (in the
+files `spin.y` and `spinlex.c` of SPIN's source distribution), with
+modifications where needed.
 
 To instantiate a Promela parser:
 
 ```python
 from promela.yacc import Parser
+
+
 parser = Parser()
 ```
 
 Then Promela code, as a string, can be parsed by:
 
 ```python
 s = '''
@@ -31,58 +39,74 @@
 	int x
 	do
 	:: x = (x + 1)
 	od;
 }
 ```
 
-The parser returns the result as an abstract syntax tree using classes from the `promela.ast` module.
+The parser returns the result as an abstract syntax tree using classes from
+the `promela.ast` module.
 The top production rule returns a `Program` instance, which itself is a `list`.
 The contents of this list
 
-There are two categories of AST classes: those that represent control flow constructs:
+There are two categories of AST classes: those that represent control
+flow constructs:
 
-- `Proctype`, (`Init`, `NeverClaim`), `Node`, (`Expression`, `Assignment`, `Assert`, `Options` (if, do), `Else`, `Break`, `Goto`, `Label`, `Call`, `Return`, `Run`), `Sequence`
+- `Proctype`, (`Init`, `NeverClaim`), `Node`, (`Expression`, `Assignment`,
+  `Assert`, `Options` (if, do), `Else`, `Break`, `Goto`, `Label`, `Call`,
+  `Return`, `Run`), `Sequence`
 
 and those that represent only syntax inside an expression:
 
 - `Terminal`, (`VarRef`, `Integer`, `Bool`), `Operator`, (`Binary`, `Unary`)
 
-The classes in parentheses are subclasses of the last class preceding the parentheses.
-Each control flow class has a method `to_pg` that recursively converts the abstract syntax tree to a program graph.
-
-A program graph is a directed graph whose edges are labeled with statements from the program.
-Nodes represent states of the program.
-Note the difference with a control flow graph, whose nodes are program statements and edges are program states.
-AST node classes correspond to nodes of the control flow graph and edges of the program graph (possibly with branching).
-
-For some node classes like `Expression` and `Assignment`, the `to_pg` method returns themselves, a.
-Almost all statements are represented as either an `Expression` or an `Assignment`.
-These label edges in the program graph, using the edge attribute `"stmt"`.
-
-The program graph is represented as a [multi-digraph](http://en.wikipedia.org/wiki/Multigraph) using [`networkx.MultiDiGraph`](https://networkx.github.io/documentation/latest/reference/classes.multidigraph.html).
-A multi-digraph is necessary, because two nodes in the program graph may be connected by two edges, each edge labeled with a different statement.
+The classes in parentheses are subclasses of the last class preceding the
+parentheses. Each control flow class has a method `to_pg` that recursively
+converts the abstract syntax tree to a program graph.
+
+A program graph is a directed graph whose edges are labeled with statements
+from the program. Nodes represent states of the program.
+Note the difference with a control flow graph, whose nodes are program
+statements and edges are program states. AST node classes correspond to nodes
+of the control flow graph and edges of the program graph (possibly with
+branching).
+
+For some node classes like `Expression` and `Assignment`, the `to_pg` method
+returns themselves, a. Almost all statements are represented as either an
+`Expression` or an `Assignment`. These label edges in the program graph,
+using the edge attribute `"stmt"`.
+
+The program graph is represented as a [multi-digraph](
+    https://en.wikipedia.org/wiki/Multigraph)
+using [`networkx.MultiDiGraph`](
+    https://networkx.org/documentation/latest/reference/classes/multidigraph.html).
+A multi-digraph is necessary, because two nodes in the program graph may be
+connected by two edges, each edge labeled with a different statement.
 For example, this is the case in the code fragment:
 
 ```promela
 bit x;
 do
 :: x == 0
 :: x == 1
 od
 ```
 
-The above defines a program graph with a single node and two self-loops, one labeled with the statement `x == 0` and another with the statement `x == 1`.
-These two statements here are guards, so they only determine whether the edge can be traversed, without affecting the program's data state (variable values).
+The above defines a program graph with a single node and two self-loops, one
+labeled with the statement `x == 0` and another with the statement `x == 1`.
+These two statements here are guards, so they only determine whether the edge
+can be traversed, without affecting the program's data state (variable values).
 
-Program graph nodes are labeled with a `"context"` attribute that can take the values:
+Program graph nodes are labeled with a `"context"` attribute that can take
+the values:
 - `"atomic"`
 - `"d_step"`
 - `None`
-The values `"atomic"` and `"d_step"` signify that the state is inside an atomic or deterministic step block.
+The values `"atomic"` and `"d_step"` signify that the state is inside an
+atomic or deterministic step block.
 
 Continuing our earlier example:
 
 ```python
 >>> g = program[0].to_pg()
 >>> g.nodes(data=True)
 [(0, {'context': None}), (1, {'context': None})]
```

### Comparing `promela-0.0.3/promela/ast.py` & `promela-0.0.4/promela/ast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Abstract syntax tree for Promela."""
-from __future__ import absolute_import
-from __future__ import division
 import logging
 import copy
 import ctypes
 import pprint
+import subprocess as _sbp
+
 import networkx as nx
 from networkx.utils import misc
 
 
 logger = logging.getLogger(__name__)
 DATATYPES = {
     'bit': ctypes.c_bool,
@@ -27,29 +27,29 @@
     """Return a fresh integer to be used as node."""
     global N
     N += 1
     return N
 
 
 def _indent(s, depth=1, skip=0):
-    w = []
+    w = list()
     for i, line in enumerate(s.splitlines()):
         indent = '' if i < skip else depth * '\t'
         w.append(indent + line)
     return '\n'.join(w)
 
 
 def to_str(x):
     try:
         return x.to_str()
     except AttributeError:
         return str(x)
 
 
-class Proctype(object):
+class Proctype:
     def __init__(self, name, body, args=None,
                  active=None, d_proc=False,
                  priority=None, provided=None):
         self.name = name
         self.body = body
         self.args = args
         if active is None:
@@ -59,25 +59,24 @@
         if priority is not None:
             priority = int(priority.value)
         self.active = active
         self.priority = priority
         self.provided = provided
 
     def __str__(self):
-        return "Proctype('{name}')".format(name=self.name)
+        return f"Proctype('{self.name}')"
 
     def to_str(self):
+        active = self._active_str()
+        args = self._args_str()
+        body = _indent(to_str(self.body))
         return (
-            '{active} proctype {name}({args}){{\n'
-            '{body}\n'
-            '}}\n\n').format(
-                active=self._active_str(),
-                name=self.name,
-                args=self._args_str(),
-                body=_indent(to_str(self.body)))
+            f'{active} proctype {self.name}({args}){{\n'
+            f'{body}\n'
+            '}}\n\n')
 
     def _active_str(self):
         if self.active is None:
             active = ''
         else:
             active = 'active [' + to_str(self.active) + '] '
         return active
@@ -88,15 +87,16 @@
         else:
             args = to_str(self.args)
         return args
 
     def to_pg(self, syntactic_else=False):
         """Return program graph of proctype.
 
-        @param syntactic_else: if `True`, then "else"
+        @param syntactic_else:
+            if `True`, then "else"
             statements in directly nested "if" or "do"
             take precedence based on syntactic context.
             The Promela language reference defines
             "else" semantically, with respect to
             the program graph.
         """
         global N
@@ -128,26 +128,31 @@
         if not syntactic_else:
             semantic_else(h)
         return h
 
 
 def contract_goto_edges(g, u):
     """Identify nodes connected with `goto` edge."""
-    assert u in g
-    assert g.root in g
+    if u not in g:
+        raise AssertionError(u)
+    if g.root not in g:
+        raise AssertionError(g.root)
     n = g.out_degree(u)
     if n == 0 or 1 < n:
         return
-    assert n == 1, n
+    if n != 1:
+        raise AssertionError(n)
     # single outgoing edge: safe to contract
     _, q, d = next(iter(g.edges(u, data=True)))
     if d['stmt'] != 'goto':
         return
     # goto
-    assert u != q, 'loop of `goto`s detected'
+    if u == q:
+        raise AssertionError(
+            'loop of `goto`s detected')
     # the source node context (atomic or d_step) is overwritten
     for p, _, d in g.in_edges(u, data=True):
         g.add_edge(p, q, **d)
     # but the source node label is preserved
     u_label = g.nodes[u].get('labels')
     if u_label is not None:
         g.nodes[q].setdefault('labels', set()).update(u_label)
@@ -161,21 +166,25 @@
     # branch node cannot have goto
     # `goto` and `break` must have transformed to `true`
     # labels must have raised `Exception`
     for u in g:
         if g.out_degree(u) <= 1:
             continue
         for _, v, d in g.edges(u, data=True):
-            assert 'stmt' in d
+            if 'stmt' not in d:
+                raise AssertionError(d)
             stmt = d['stmt']
-            assert stmt != 'goto', stmt
+            if stmt == 'goto':
+                raise AssertionError(stmt)
     for u, d in g.nodes(data=True):
-        assert 'context' in d
+        if 'context' not in d:
+            raise AssertionError(d)
     for u, v, d in g.edges(data=True):
-        assert 'stmt' in d
+        if 'stmt' not in d:
+            raise AssertionError(d)
 
 
 def map_uuid_to_int(g):
     """Reinplace uuid nodes with integers."""
     umap = {u: i for i, u in enumerate(sorted(g, key=str))}
     h = nx.MultiDiGraph(name=g.name)
     for u, d in g.nodes(data=True):
@@ -223,37 +232,38 @@
 
 class Program(list):
     def __str__(self):
         return '\n'.join(to_str(x) for x in self)
 
     def __repr__(self):
         c = super(Program, self).__repr__()
-        return 'Program({c})'.format(c=c)
+        return f'Program({c})'
 
     def to_table(self):
         """Return global definitions, proctypes, and LTL blocks.
 
-        @rtype: 3-`tuple` of `set`
+        @rtype:
+            3-`tuple` of `set`
         """
         units = misc.flatten(self)
         ltl = {x for x in units if isinstance(x, LTL)}
         proctypes = {x for x in units if isinstance(x, Proctype)}
         global_defs = {x for x in units
                        if x not in proctypes and x not in ltl}
         return global_defs, proctypes, ltl
 
 
-class LTL(object):
+class LTL:
     """Used to mark strings as LTL blocks."""
 
     def __init__(self, formula):
         self.formula = formula
 
     def __repr__(self):
-        return 'LTL({f})'.format(f=repr(self.formula))
+        return f'LTL({self.formula!r})'
 
     def __str__(self):
         return 'ltl {' + str(self.formula) + '}'
 
 
 class Sequence(list):
     def __init__(self, iterable, context=None, is_option=False):
@@ -268,31 +278,36 @@
         else:
             return (
                 self.context + '{\n' +
                 _indent(to_str(self)) + '\n}\n')
 
     def __repr__(self):
         l = super(Sequence, self).__repr__()
-        return 'Sequence({l}, context={c}, is_option={isopt})'.format(
-            l=l, c=self.context, isopt=self.is_option)
+        return (
+            f'Sequence({l}, '
+            f'context={self.context}, '
+            f'is_option={self.is_option})')
 
     def to_pg(self, g, context=None, option_guard=None, **kw):
         # set context
         if context is None:
             context = self.context
         c = context
-        assert c in {'atomic', 'd_step', None}
+        if c not in {'atomic', 'd_step', None}:
+            raise AssertionError(c)
         # atomic cannot appear inside d_step
         if context == 'd_step' and c == 'atomic':
             raise Exception('atomic inside d_step')
         context = c
         # find first non-decl
         # option guard first
         option_guard = self.is_option or option_guard
-        assert len(self) > 0
+        len_self = len(self)
+        if len_self <= 0:
+            raise AssertionError(len_self)
         stmts = iter(self)
         t = None
         for stmt in stmts:
             t = stmt.to_pg(g, context=context,
                            option_guard=option_guard, **kw)
             if t is not None:
                 break
@@ -300,33 +315,36 @@
         if t is None:
             return None
         e, tail = t
         # guard can't be a goto or label
         # (should have been caught below)
         if option_guard:
             for u, d in e:
-                assert d.get('stmt') != 'goto', self
+                if d.get('stmt') == 'goto':
+                    raise AssertionError(self)
         # other option statements
         for stmt in stmts:
             t = stmt.to_pg(g, context=context, option_guard=None, **kw)
             # decl ?
             if t is None:
                 continue
             ine, out = t
             # connect tail to ine
-            assert ine
+            if not ine:
+                raise AssertionError(ine)
             for v, d in ine:
                 g.add_edge(tail, v, **d)
             # update tail
-            assert out in g
+            if out not in g:
+                raise AssertionError(out)
             tail = out
         return e, tail
 
 
-class Node(object):
+class Node:
     def to_pg(self, g, context=None, **kw):
         u = generate_unique_node()
         g.add_node(u, context=context)
         e = (u, dict(stmt=self))
         return [e], u
 
 
@@ -339,73 +357,80 @@
         a, b = self.entry_exit
         c = list()
         c.append(a)
         c.append('\n')
         for option in self.options:
             option_guard = _indent(to_str(option[0]), skip=1)
             w = [_indent(to_str(x)) for x in option[1:]]
-            c.append(
-                ':: {option_guard}{tail}\n'.format(
-                    option_guard=option_guard,
-                    tail=(' ->\n' + '\n'.join(w)) if w else ''))
+            tail = (' ->\n' + '\n'.join(w)) if w else ''
+            c.append(f':: {option_guard}{tail}\n')
         c.append(b)
         c.append(';\n')
         return ''.join(c)
 
     @property
     def entry_exit(self):
         if self.type == 'if':
             return ('if', 'fi')
         elif self.type == 'do':
             return ('do', 'od')
 
     def to_pg(self, g, od_exit=None,
               context=None, option_guard=None,
               syntactic_else=False, **kw):
-        logger.info('-- start flattening {t}'.format(t=self.type))
-        assert self.options
-        assert self.type in {'if', 'do'}
+        logger.info(f'-- start flattening {self.type}')
+        if not self.options:
+            raise AssertionError(self.options)
+        if self.type not in {'if', 'do'}:
+            raise AssertionError(self.type)
         # create target
         target = generate_unique_node()
         g.add_node(target, context=context)
         # target != exit node ?
         if self.type == 'do':
             od_exit = generate_unique_node()
             g.add_node(od_exit, context=context)
         self_else = None
         self_has_else = False
         option_has_else = False
         edges = list()
         else_ine = None
         for option in self.options:
-            logger.debug('option: {opt}'.format(opt=option))
+            logger.debug(f'option: {option}')
             t = option.to_pg(g, od_exit=od_exit, context=context, **kw)
-            assert t is not None  # decls filtered by `Sequence`
+            # decls filtered by `Sequence`
+            if t is None:
+                raise AssertionError(t)
             ine, out = t
-            assert out in g
+            if out not in g:
+                raise AssertionError(out)
             # detect `else`
             has_else = False
             for u, d in ine:
                 stmt = d.get('stmt')
                 if isinstance(stmt, Else):
                     has_else = True
                     self_else = stmt
                 # option cannot start with goto (= contraction)
-                assert stmt != 'goto'
+                if stmt == 'goto':
+                    raise AssertionError(stmt)
             # who owns this else ?
             if has_else:
                 if len(ine) == 1:
-                    assert not self_has_else, option
+                    if self_has_else:
+                        raise AssertionError(option)
                     self_has_else = True
                     if not syntactic_else:
-                        assert not option_has_else, option
+                        if option_has_else:
+                            raise AssertionError(option)
                 elif len(ine) > 1:
                     option_has_else = True
                     if not syntactic_else:
-                        assert not self_has_else, option
+                        if self_has_else:
+                            raise AssertionError(option)
                 else:
                     raise Exception('option with no in edges')
             # collect in edges, except for own `else`
             if not (has_else and self_has_else):
                 edges.extend(ine)
             else:
                 else_ine = ine  # keep for later
@@ -424,27 +449,27 @@
             edges.extend(else_ine)
         # what is the exit node ?
         if self.type == 'if':
             out = target
         elif self.type == 'do':
             out = od_exit
         else:
-            raise Exception('Unknown type: {t}'.format(t=out))
+            raise Exception(f'Unknown type: {out}')
         # is not itself an option guard ?
         if option_guard:
             logger.debug('is option guard')
         if self.type == 'do' and option_guard is None:
             edge = (target, dict(stmt='goto'))
             in_edges = [edge]
         else:
             in_edges = edges
-        logger.debug('in edges: {ie}, out: {out}\n'.format(
-            ie=in_edges, out=out))
-        logger.info('-- end flattening {t}'.format(t=self.type))
-        assert out in g
+        logger.debug(f'in edges: {in_edges}, out: {out}\n')
+        logger.info(f'-- end flattening {self.type}')
+        if out not in g:
+            raise AssertionError(out)
         return in_edges, out
 
 
 class Else(Node):
     def __init__(self):
         self.other_guards = None
 
@@ -457,36 +482,38 @@
         return 'break'
 
     def to_pg(self, g, od_exit=None, **kw):
         if od_exit is None:
             raise Exception('Break outside repetition construct.')
         # like goto, but with: v = od_exit
         # context of od_tail is determined by do loop
-        assert od_exit in g
+        if od_exit not in g:
+            raise AssertionError(od_exit)
         v = od_exit
         return goto_to_pg(g, v, **kw)
 
 
 class Goto(Node):
     def __init__(self, label):
         self.label = label
 
     def __str__(self):
-        return 'goto {l}'.format(l=self.label)
+        return f'goto {self.label}'
 
     def to_pg(self, g, context=None, **kw):
         v = _format_label(self.label)
         # ok, because source node context
         # is overwritten during contraction
         g.add_node(v, context=context)
         return goto_to_pg(g, v, context=context, **kw)
 
 
 def goto_to_pg(g, v, option_guard=None, context=None, **kw):
-    assert v in g
+    if v not in g:
+        raise AssertionError(v)
     if option_guard is None:
         stmt = 'goto'
     else:
         stmt = Bool('true')
     e = (v, dict(stmt=stmt))
     u = generate_unique_node()
     g.add_node(u, context=context)
@@ -495,38 +522,39 @@
 
 class Label(Node):
     def __init__(self, label, body):
         self.label = label
         self.body = body
 
     def to_str(self):
-        return '{l}: {b}'.format(l=self.label, b=to_str(self.body))
+        return f'{self.label}: {to_str(self.body)}'
 
     def to_pg(self, g, option_guard=None, context=None, **kw):
         if option_guard is not None:
             raise Exception('option guard cannot be labeled')
         # add label node, with context
         u = _format_label(self.label)
         g.add_node(u, context=context, labels={self.label})
         # flatten body
         t = self.body.to_pg(g, context=context, **kw)
         if t is None:
             raise Exception('Label of variable declaration.')
         ine, out = t
-        assert out in g
+        if out not in g:
+            raise AssertionError(out)
         # make ine out edges of label node
         for v, d in ine:
             g.add_edge(u, v, **d)
         # appear like a goto (almost)
         e = (u, dict(stmt='goto'))
         return [e], out
 
 
 def _format_label(label):
-    return 'label_{l}'.format(l=label)
+    return f'label_{label}'
 
 
 # TODO: check that referenced types exist, before adding typedef
 # to symbol table
 
 class VarDef(Node):
     def __init__(self, name, vartype, length=None,
@@ -534,53 +562,56 @@
                  msg_types=None, initval=None):
         self.name = name
         self.type = vartype
         if length is None:
             l = None
         else:
             l = eval(str(length))
-            assert isinstance(l, int), l
+            if not isinstance(l, int):
+                raise AssertionError(l)
         self.length = l
         self.visible = visible
         if bitwidth is not None:
             self.bitwidth = int(bitwidth.value)
         if vartype == 'bool':
             default_initval = Bool('false')
         else:
             default_initval = Integer('0')
         if initval is None:
             initval = Expression(default_initval)
         self.initial_value = initval
         # TODO message types
 
     def __repr__(self):
-        return 'VarDef({t}, {v})'.format(t=self.type, v=self.name)
+        return f'VarDef({self.type}, {self.name})'
 
     def to_str(self):
-        s = '{type} {varname}{len}'.format(
-            type=self._type_str(),
-            varname=self.name,
-            len='[{n}]'.format(n=self.len) if self.len else '')
+        type = self._type_str()
+        varname = self.name
+        length = f'[{self.len}]' if self.len else ''
+        s = f'{type} {varname}{length}'
         return s
 
     def _type_str(self):
         return self.type
 
     def to_pg(self, g, **kw):
         # var declarations are collected before the process runs
         # man page: datatypes, p.405
         g.locals.add(self)
         return None
 
     def insert(self, symbol_table, pid):
         """Insert variable into table of symbols.
 
-        @type symbol_table: L{SymbolTable}
-
-        @type pid: int or None
+        @type symbol_table:
+            `SymbolTable`
+        @type pid:
+            int or
+            None
         """
         t = self.type
         if t == 'chan':
             v = MessageChannel(self.len)
             # channels are always available globally
             # note how this differs from having global scope:
             # no name conflicts
@@ -599,29 +630,28 @@
                 _fields_ = [('value', ctypes.c_uint, n)]
 
             if self.len is None:
                 v = Unsigned()
             else:
                 v = [Unsigned() for i in range(self.len)]
         else:
-            raise TypeError('unknown type "{t}"'.format(t=t))
+            raise TypeError(f'unknown type "{t}"')
         # global scope ?
         if pid is None:
             d = symbol_table.globals
         else:
             d = symbol_table.locals[pid]
         name = self.name
         if name in d:
-            raise Exception('variable "{name}" is already defined'.format(
-                            name=name))
+            raise Exception(f'variable "{name}" is already defined')
         else:
             d[name] = v
 
 
-class SymbolTable(object):
+class SymbolTable:
     """Variable, user data and message type definitions.
 
     Attributes:
 
       - `globals`: `dict` of global vars
       - `locals`: `dict` of `dicts`, keys of outer `dict` are pids
       - `channels`: `dict` of global lists for channels
@@ -675,27 +705,22 @@
             if d['name'] != q['name']:
                 return False
             if d['pc'] != q['pc']:
                 return False
         return True
 
     def __str__(self):
+        pids = pprint.pformat(self.pids, width=15)
         return (
-            'globals: {g}\n'
-            'channels: {c}\n'
-            'pids: {p}\n\n'
-            'types: {t}\n'
-            'locals: {l}\n'
-            'exclusive: {e}\n').format(
-                g=self.globals,
-                l=self.locals,
-                p=pprint.pformat(self.pids, width=15),
-                t=self.types,
-                e=self.exclusive,
-                c=self.channels)
+            f'globals: {self.globals}\n'
+            f'channels: {self.channels}\n'
+            f'pids: {pids}\n\n'
+            f'types: {self.types}\n'
+            f'locals: {self.locals}\n'
+            f'exclusive: {self.exclusive}\n')
 
     def copy(self):
         new = SymbolTable()
         # auxiliary
         new.exclusive = self.exclusive
         new.handshake = self.handshake
         new.timeout = self.timeout
@@ -708,25 +733,24 @@
         new.pids = {k: {'name': d['name'],
                         'pc': d['pc']}
                     for k, d in self.pids.items()}
         new.types = self.types
         return new
 
 
-class MessageChannel(object):
+class MessageChannel:
     def __init__(self, nslots):
         self.nslots = nslots
         self.contents = list()
 
     def send(self, x):
         if len(self.contents) < self.nslots:
             self.contents.append(x)
         else:
-            raise Exception('channel {name} is full'.format(
-                            name=self.name))
+            raise Exception(f'channel {self.name} is full')
 
     def receive(self, x=None, random=False, rm=True):
         c = self.contents
         i = 0
         if x and random:
             i = c.index(x)
         m = c[i]
@@ -737,27 +761,27 @@
 
 class TypeDef(Node):
     def __init__(self, name, decls):
         self.name = name
         self.decls = decls
 
     def __str__(self):
-        return 'typedef {name} {\ndecls\n}'.format(
-            name=self.name, decls=to_str(self.decls))
+        decls = to_str(self.decls)
+        return f'typedef {self.name} {decls}'
 
     def exe(self, t):
         t.types[self.name] = self
 
 
 class MessageType(Node):
     def __init__(self, values, visible=None):
         self.values = values
 
     def __str__(self):
-        return 'mtype {{ {values} }}'.format(values=self.values)
+        return f'mtype {{ {self.values} }}'
 
     def exe(self, t):
         t.types[self.name] = self
 
 
 class Return(Node):
     def __init__(self, expr):
@@ -770,15 +794,15 @@
 class Run(Node):
     def __init__(self, func, args=None, priority=None):
         self.func = func
         self.args = args
         self.priority = priority
 
     def __str__(self):
-        return 'run({f})'.format(f=self.func)
+        return f'run({self.func})'
 
 
 class Inline(Node):
     def __init__(self, name, args):
         self.name = name
         self.args = args
 
@@ -790,23 +814,23 @@
 
 
 class Assert(Node):
     def __init__(self, expr):
         self.expr = expr
 
     def __repr__(self):
-        return 'assert({expr})'.format(expr=repr(self.expr))
+        return f'assert({self.expr!r})'
 
 
 class Expression(Node):
     def __init__(self, expr):
         self.expr = expr
 
     def __repr__(self):
-        return 'Expression({expr})'.format(expr=repr(self.expr))
+        return f'Expression({self.expr!r})'
 
     def __str__(self):
         return to_str(self.expr)
 
     def eval(self, g, l):
         s = str(self)
         g = dict(g)
@@ -832,23 +856,21 @@
 
 class Assignment(Node):
     def __init__(self, var, value):
         self.var = var
         self.value = value
 
     def __repr__(self):
-        return 'Assignment({var}, {val})'.format(
-            var=repr(self.var), val=repr(self.value))
+        return f'Assignment({self.var!r}, {self.value!r})'
 
     def __str__(self):
-        return '{var} = {val}'.format(var=self.var, val=self.value)
+        return f'{self.var} = {self.value}'
 
     def exe(self, g, l):
-        logger.debug('Assign: {var} = {val}'.format(
-                     var=self.var, val=self.value))
+        logger.debug(f'Assign: {self.var} = {self.value}')
         s = self.to_str()
         og = g
         ol = l
         g = dict(g)
         for k, v in g.items():
             if 'ctypes' in str(type(v)):
                 g[k] = int(v.value)
@@ -874,72 +896,69 @@
 class Receive(Node):
     def __init__(self, varref, args=None):
         self.var = varref
         self.args = args
 
     def __str__(self):
         v = to_str(self.var)
-        return 'Rx({v})'.format(v=v)
+        return f'Rx({v})'
 
 
 class Send(Node):
     def __init__(self, varref, args=None):
         self.varref = varref
         self.args = args
 
     def __str__(self):
         v = to_str(self.var)
-        return 'Tx({v})'.format(v=v)
+        return f'Tx({v})'
 
 
 class Printf(Node):
     def __init__(self, s, args):
         self.s = s
         self.args = args
 
     def __str__(self):
-        return 'printf()'.format(s=self.s, args=self.args)
+        args = ', '.join(self.args)
+        return f'printf({self.s}, {args})'
 
 
-class Operator(object):
+class Operator:
     def __init__(self, operator, *operands):
         self.operator = operator
         self.operands = operands
 
     def __repr__(self):
-        return 'Operator({op}, {xy})'.format(
-            op=repr(self.operator),
-            xy=', '.join(repr(x) for x in self.operands))
+        xy = ', '.join(repr(x) for x in self.operands)
+        return f'Operator({self.operator!r}, {xy})'
 
     def __str__(self):
-        return '({op} {xy})'.format(
-            op=self.operator,
-            xy=' '.join(to_str(x) for x in self.operands))
+        xy = ' '.join(to_str(x) for x in self.operands)
+        return f'({self.operator} {xy})'
 
 
 class Binary(Operator):
     def __str__(self):
-        return '({x} {op} {y})'.format(
-            x=to_str(self.operands[0]),
-            op=self.operator,
-            y=to_str(self.operands[1]))
+        x = to_str(self.operands[0])
+        y = to_str(self.operands[1])
+        return f'({x} {self.operator} {y})'
+
 
 
 class Unary(Operator):
     pass
 
 
-class Terminal(object):
+class Terminal:
     def __init__(self, value):
         self.value = value
 
     def __repr__(self):
-        return '{classname}({val})'.format(
-            classname=type(self).__name__,
-            val=repr(self.value))
+        return f'{type(self).__name__}({self.value!r})'
 
     def __str__(self):
         return str(self.value)
 
 
 class VarRef(Terminal):
     def __init__(self, name, index=None, extension=None):
@@ -950,28 +969,23 @@
             i = index
         self.index = i
         self.extension = extension
         # used by some external methods
         self.value = name
 
     def __repr__(self):
-        return 'VarRef({name}, {index}, {ext})'.format(
-            name=repr(self.name),
-            index=repr(self.index),
-            ext=repr(self.extension))
+        return f'VarRef({self.name!r}, {self.index!r}, {self.extension!r})'
 
     def __str__(self):
         if self.index is None:
-            i = ''
+            index = ''
         else:
-            i = '[{i}]'.format(i=to_str(self.index))
-        return '{name}{index}{ext}'.format(
-            name=self.name,
-            index=i,
-            ext='' if self.extension is None else self.extension)
+            index = f'[{to_str(self.index)}]'
+        ext = '' if self.extension is None else self.extension
+        return f'{self.name}{index}{ext}'
 
 
 class Integer(Terminal):
     def __bool__(self):
         return bool(int(self.value))
 
 
@@ -979,57 +993,78 @@
     def __init__(self, val):
         self.value = val.upper() == 'TRUE'
 
     def __bool__(self):
         return self.value
 
     def __repr__(self):
-        return 'Bool({value})'.format(value=repr(self.value))
+        return f'Bool({self.value!r})'
 
     def __str__(self):
         return str(self.value)
 
 
 class RemoteRef(Terminal):
     def __init__(self, proctype, label, pid=None):
         self.proctype = proctype
         self.label = label
         self.pid = pid
 
     def __repr__(self):
-        return 'RemoteRef({proc}, {label}, {pid})'.format(
-            proc=self.proctype, label=self.label, pid=self.pid)
+        return f'RemoteRef({self.proctype}, {self.label}, {self.pid})'
 
     def __str__(self):
         if self.pid is None:
             inst = ''
         else:
-            inst = '[{pid}]'.format(pid=self.pid)
-        return '{proc} {inst} @ {label}'.format(
-            proc=self.proctype, inst=inst, label=self.label)
+            inst = f'[{self.pid}]'
+        return f'{self.proctype} {inst} @ {self.label}'
 
 
 def dump_graph(g, fname='a.pdf', node_label='label',
                edge_label='label', relabel=False):
     """Write the program graph, annotated with formulae, to PDF file."""
     # map nodes to integers
     if relabel:
         mapping = {u: i for i, u in enumerate(g)}
         g = nx.relabel_nodes(g, mapping)
         inv_mapping = {v: k for k, v in mapping.items()}
         s = list()
         s.append('mapping of nodes:')
         for k in sorted(inv_mapping):
             v = inv_mapping[k]
-            s.append('{k}: {v}'.format(k=k, v=v))
+            s.append(f'{k}: {v}')
         print('\n'.join(s))
     h = nx.MultiDiGraph()
     for u, d in g.nodes(data=True):
         label = d.get(node_label, u)
-        label = '"{label}"'.format(label=label)
+        label = f'"{label}"'
         h.add_node(u, label=label)
     for u, v, d in g.edges(data=True):
         label = d.get(edge_label, ' ')
-        label = '"{label}"'.format(label=label)
+        label = f'"{label}"'
         h.add_edge(u, v, label=label)
-    pd = nx.drawing.nx_pydot.to_pydot(h)
-    pd.write_pdf(fname)
+    # format as DOT
+    nodes = list()
+    for u, d in h.nodes(data=True):
+        label = d['label']
+        nodes.append(
+            f'{u} [label={label}];')
+    nodes_dot = '\n'.join(nodes)
+    edges = list()
+    for u, v, d in h.edges(data=True):
+        label = d['label']
+        edges.append(
+            f'{u} -> {v} [label={label}];')
+    edges_dot = '\n'.join(edges)
+    dot_text = f'digraph {{ {nodes_dot}\n{edges_dot} }}'
+    # write as PDF
+    dot = [
+        'dot',
+        '-Tpdf',
+        f'-o{fname}']
+    _sbp.run(
+        dot,
+        encoding='utf8',
+        input=dot_text,
+        capture_output=True,
+        check=True)
```

### Comparing `promela-0.0.3/promela/lex.py` & `promela-0.0.4/promela/lex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,211 +1,229 @@
 """Lexer for Promela, using Python Lex-Yacc (PLY)."""
 import logging
+
 import ply.lex
 
 
 logger = logging.getLogger(__name__)
 
 
-class Lexer(object):
+class Lexer:
     """Lexer for the Promela modeling language."""
 
-    states = tuple([('ltl', 'inclusive')])
-    reserved = {
-        '_np': 'NONPROGRESS',
-        'true': 'TRUE',
-        'false': 'FALSE',
-        'active': 'ACTIVE',
-        'assert': 'ASSERT',
-        'atomic': 'ATOMIC',
-        'bit': 'BIT',
-        'bool': 'BOOL',
-        'break': 'BREAK',
-        'byte': 'BYTE',
-        'chan': 'CHAN',
-        'd_step': 'D_STEP',
-        'd_proctype': 'D_PROCTYPE',
-        'do': 'DO',
-        'else': 'ELSE',
-        'empty': 'EMPTY',
-        'enabled': 'ENABLED',
-        'eval': 'EVAL',
-        'fi': 'FI',
-        'full': 'FULL',
-        'get_priority': 'GET_P',
-        'goto': 'GOTO',
-        'hidden': 'HIDDEN',
-        'if': 'IF',
-        'init': 'INIT',
-        'int': 'INT',
-        'len': 'LEN',
-        'local': 'ISLOCAL',
-        'ltl': 'LTL',
-        'mtype': 'MTYPE',
-        'nempty': 'NEMPTY',
-        'never': 'CLAIM',
-        'nfull': 'NFULL',
-        'od': 'OD',
-        'of': 'OF',
-        'pc_value': 'PC_VAL',
-        'pid': 'PID',
-        'printf': 'PRINT',
-        'priority': 'PRIORITY',
-        'proctype': 'PROCTYPE',
-        'provided': 'PROVIDED',
-        'R': 'RELEASE',
-        'return': 'RETURN',
-        'run': 'RUN',
-        'short': 'SHORT',
-        'skip': 'TRUE',
-        'show': 'SHOW',
-        'timeout': 'TIMEOUT',
-        'typedef': 'TYPEDEF',
-        'U': 'UNTIL',
-        'unless': 'UNLESS',
-        'unsigned': 'UNSIGNED',
-        'X': 'NEXT',
-        'xr': 'XR',
-        'xs': 'XS',
-        'W': 'WEAK_UNTIL'}
-    values = {'skip': 'true'}
-    delimiters = ['LPAREN', 'RPAREN', 'LBRACKET', 'RBRACKET',
-                  'LBRACE', 'RBRACE', 'COMMA', 'PERIOD',
-                  'SEMI', 'COLONS', 'COLON', 'ELLIPSIS']
-    # remember to check precedence
-    operators = ['PLUS', 'INCR', 'MINUS', 'DECR', 'TIMES', 'DIVIDE',
-                 'MOD', 'OR', 'AND', 'NOT', 'XOR', 'IMPLIES', 'EQUIV',
-                 'LOR', 'LAND', 'LNOT', 'LT', 'GT',
-                 'LE', 'GE', 'EQ', 'NE',
-                 'RCV', 'R_RCV', 'TX2', 'LSHIFT', 'RSHIFT', 'AT',
-                 'ALWAYS', 'EVENTUALLY']
-    misc = ['EQUALS', 'ARROW', 'STRING', 'NAME', 'INTEGER',
-            'PREPROC', 'NEWLINE', 'COMMENT']
-
     def __init__(self, debug=False):
+        self.states = tuple([('ltl', 'inclusive')])
+        self.reserved = {
+            '_np': 'NONPROGRESS',
+            'true': 'TRUE',
+            'false': 'FALSE',
+            'active': 'ACTIVE',
+            'assert': 'ASSERT',
+            'atomic': 'ATOMIC',
+            'bit': 'BIT',
+            'bool': 'BOOL',
+            'break': 'BREAK',
+            'byte': 'BYTE',
+            'chan': 'CHAN',
+            'd_step': 'D_STEP',
+            'd_proctype': 'D_PROCTYPE',
+            'do': 'DO',
+            'else': 'ELSE',
+            'empty': 'EMPTY',
+            'enabled': 'ENABLED',
+            'eval': 'EVAL',
+            'fi': 'FI',
+            'full': 'FULL',
+            'get_priority': 'GET_P',
+            'goto': 'GOTO',
+            'hidden': 'HIDDEN',
+            'if': 'IF',
+            'init': 'INIT',
+            'int': 'INT',
+            'len': 'LEN',
+            'local': 'ISLOCAL',
+            'ltl': 'LTL',
+            'mtype': 'MTYPE',
+            'nempty': 'NEMPTY',
+            'never': 'CLAIM',
+            'nfull': 'NFULL',
+            'od': 'OD',
+            'of': 'OF',
+            'pc_value': 'PC_VAL',
+            'pid': 'PID',
+            'printf': 'PRINT',
+            'priority': 'PRIORITY',
+            'proctype': 'PROCTYPE',
+            'provided': 'PROVIDED',
+            'R': 'RELEASE',
+            'return': 'RETURN',
+            'run': 'RUN',
+            'short': 'SHORT',
+            'skip': 'TRUE',
+            'show': 'SHOW',
+            'timeout': 'TIMEOUT',
+            'typedef': 'TYPEDEF',
+            'U': 'UNTIL',
+            'unless': 'UNLESS',
+            'unsigned': 'UNSIGNED',
+            'X': 'NEXT',
+            'xr': 'XR',
+            'xs': 'XS',
+            'W': 'WEAK_UNTIL'}
+        self.values = {'skip': 'true'}
+        self.delimiters = [
+            'LPAREN', 'RPAREN', 'LBRACKET', 'RBRACKET',
+            'LBRACE', 'RBRACE', 'COMMA', 'PERIOD',
+            'SEMI', 'COLONS', 'COLON', 'ELLIPSIS']
+        # remember to check precedence
+        self.operators = [
+            'PLUS', 'INCR', 'MINUS', 'DECR', 'TIMES', 'DIVIDE',
+            'MOD', 'OR', 'AND', 'NOT', 'XOR', 'IMPLIES', 'EQUIV',
+            'LOR', 'LAND', 'LNOT', 'LT', 'GT',
+            'LE', 'GE', 'EQ', 'NE',
+            'RCV', 'R_RCV', 'TX2', 'LSHIFT', 'RSHIFT', 'AT',
+            'ALWAYS', 'EVENTUALLY']
+        self.misc = [
+            'EQUALS', 'ARROW', 'STRING', 'NAME', 'INTEGER',
+            'PREPROC', 'NEWLINE', 'COMMENT']
         self.tokens = (
             self.delimiters + self.operators +
-            self.misc + list(set(self.reserved.values())))
+            self.misc + sorted(set(self.reserved.values())))
         self.build(debug=debug)
 
     def build(self, debug=False, debuglog=None, **kwargs):
         """Create a lexer.
 
-        @param kwargs: Same arguments as C{ply.lex.lex}:
+        @param kwargs: Same arguments as `ply.lex.lex`:
 
-          - except for C{module} (fixed to C{self})
-          - C{debuglog} defaults to the module's logger.
+          - except for `module` (fixed to `self`)
+          - `debuglog` defaults to the module's logger.
         """
         if debug and debuglog is None:
             debuglog = logger
         self.lexer = ply.lex.lex(
             module=self,
             debug=debug,
             debuglog=debuglog,
             **kwargs)
 
     # check for reserved words
     def t_NAME(self, t):
-        r'[a-zA-Z_][a-zA-Z_0-9]*'
+        r"""
+        [a-zA-Z_]
+        [a-zA-Z_0-9]*
+        """
         t.value = self.values.get(t.value, t.value)
         t.type = self.reserved.get(t.value, 'NAME')
         # switch to LTL context
         if t.value == 'ltl':
             self.lexer.level = 0
             self.lexer.begin('ltl')
         return t
 
     def t_STRING(self, t):
-        r'"[^"]*"'
+        r' " [^"]* " '
         return t
 
     # operators
-    t_PLUS = r'\+'
-    t_INCR = r'\+\+'
-    t_MINUS = r'-'
-    t_DECR = r'--'
-    t_TIMES = r'\*'
-    t_DIVIDE = r'/'
-    t_MOD = r'%'
-    t_OR = r'\|'
-    t_AND = r'&'
-    t_NOT = r'~'
-    t_XOR = r'\^'
-    t_LOR = r'\|\|'
-    t_LAND = r'&&'
-    t_LNOT = r'!'
-    t_TX2 = r'!!'
-    t_LT = r'<'
-    t_LSHIFT = r'<<'
-    t_GT = r'>'
-    t_RSHIFT = r'>>'
-    t_LE = r'<='
-    t_GE = r'>='
-    t_EQ = r'=='
-    t_NE = r'!='
-    t_RCV = r'\?'
-    t_R_RCV = r'\?\?'
-    t_AT = r'@'
-    t_EQUIV = r'<->'
+    t_PLUS = r' \+ '
+    t_INCR = r' \+ \+ '
+    t_MINUS = r' \- '
+    t_DECR = r' \- \- '
+    t_TIMES = r' \* '
+    t_DIVIDE = r' / '
+    t_MOD = r' % '
+    t_OR = r' \| '
+    t_AND = r' \& '
+    t_NOT = r' \~ '
+    t_XOR = r' \^ '
+    t_LOR = r' \| \| '
+    t_LAND = r' \& \& '
+    t_LNOT = r' ! '
+    t_TX2 = r' !! '
+    t_LT = r' < '
+    t_LSHIFT = r' << '
+    t_GT = r' > '
+    t_RSHIFT = r' >> '
+    t_LE = r' <= '
+    t_GE = r' >= '
+    t_EQ = r' == '
+    t_NE = r' != '
+    t_RCV = r' \? '
+    t_R_RCV = r' \? \? '
+    t_AT = r' @ '
+    t_EQUIV = r' < \- > '
     # assignment
-    t_EQUALS = r'='
+    t_EQUALS = r' = '
     # temporal operators
-    t_ALWAYS = r'\[\]'
-    t_EVENTUALLY = r'\<\>'
+    t_ALWAYS = r' \[ \] '
+    t_EVENTUALLY = r' <> '
     # delimeters
-    t_LPAREN = r'\('
-    t_RPAREN = r'\)'
-    t_LBRACKET = r'\['
-    t_RBRACKET = r'\]'
-    t_LBRACE = r'\{'
-    t_RBRACE = r'\}'
-    t_COMMA = r','
-    t_PERIOD = r'\.'
-    t_SEMI = r';'
-    t_COLONS = r'::'
-    t_COLON = r':'
-    t_ELLIPSIS = r'\.\.\.'
+    t_LPAREN = r' \( '
+    t_RPAREN = r' \) '
+    t_LBRACKET = r' \[ '
+    t_RBRACKET = r' \] '
+    t_LBRACE = r' \{ '
+    t_RBRACE = r' \} '
+    t_COMMA = r' , '
+    t_PERIOD = r' \. '
+    t_SEMI = r' ; '
+    t_COLONS = r' :: '
+    t_COLON = r' : '
+    t_ELLIPSIS = r' \. \. \. '
 
     def t_ltl_LBRACE(self, t):
-        r'\{'
+        r' \{ '
         self.lexer.level += 1
         return t
 
     def t_ltl_RBRACE(self, t):
-        r'\}'
+        r' \} '
         self.lexer.level -= 1
         if self.lexer.level == 0:
             self.lexer.begin('INITIAL')
         return t
 
     def t_ltl_ARROW(self, t):
-        r'->'
+        r' \- > '
         t.type = 'IMPLIES'
         return t
 
-    t_INITIAL_ARROW = r'->'
+    t_INITIAL_ARROW = r' \- > '
 
     def t_PREPROC(self, t):
-        r'\#.*'
+        r' \# .* '
         pass
 
     def t_INTEGER(self, t):
-        r'\d+([uU]|[lL]|[uU][lL]|[lL][uU])?'
+        r"""
+        \d+
+        (
+          [uU]
+        | [lL]
+        | [uU][lL]
+        | [lL][uU]
+        )?
+        """
         return t
 
     # t_ignore is reserved by lex to provide
     # much more efficient internal handling by lex
     #
     # A string containing ignored characters (spaces and tabs)
-    t_ignore = ' \t'
+    t_ignore = ''.join(['\x20', '\t'])
 
     def t_NEWLINE(self, t):
-        r'\n+'
+        r' \n+ '
         t.lexer.lineno += t.value.count('\n')
 
     def t_COMMENT(self, t):
-        r' /\*(.|\n)*?\*/'
+        r"""
+        / \*
+        (. | \n)*?
+        \* /
+        """
         t.lineno += t.value.count('\n')
 
     def t_error(self, t):
-        logger.error('Illegal character "{s}"'.format(s=t.value[0]))
+        logger.error(f'Illegal character "{t.value[0]}"')
         t.lexer.skip(1)
```

### Comparing `promela-0.0.3/promela/promela_parsetab.py` & `promela-0.0.4/promela/promela_parsetab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # promela_parsetab.py
 # This file is automatically generated. Do not edit.
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'programrightEQUALSleftTX2RCVR_RCVleftIMPLIESEQUIVleftLORleftLANDleftALWAYSEVENTUALLYleftUNTILWEAK_UNTILRELEASErightNEXTleftORleftXORleftANDleftEQNEleftLTLEGTGEleftLSHIFTRSHIFTleftPLUSMINUSleftTIMESDIVIDEMODleftINCRDECRrightLNOTNOTUMINUSNEGleftDOTleftLPARENRPARENLBRACKETRBRACKETLPAREN RPAREN LBRACKET RBRACKET LBRACE RBRACE COMMA PERIOD SEMI COLONS COLON ELLIPSIS PLUS INCR MINUS DECR TIMES DIVIDE MOD OR AND NOT XOR IMPLIES EQUIV LOR LAND LNOT LT GT LE GE EQ NE RCV R_RCV TX2 LSHIFT RSHIFT AT ALWAYS EVENTUALLY EQUALS ARROW STRING NAME INTEGER PREPROC NEWLINE COMMENT UNLESS TYPEDEF EVAL EMPTY NEMPTY RETURN RUN PROCTYPE OD RELEASE SHOW NONPROGRESS LTL ATOMIC TIMEOUT GET_P INIT ELSE WEAK_UNTIL UNSIGNED BREAK BIT BYTE FULL NFULL BOOL TRUE OF ASSERT ACTIVE FI XS PID SHORT FALSE IF PC_VAL PRINT XR ENABLED LEN ISLOCAL HIDDEN D_PROCTYPE MTYPE DO PROVIDED CLAIM UNTIL D_STEP CHAN INT PRIORITY NEXT GOTOprogram : unitsunits : units unitunits : unitunit : proc\n                | init\n                | claim\n                | ltl\n        unit : one_decl\n                | utype\n        unit : semiproc : prefix_proctype NAME       LPAREN decl RPAREN       opt_priority opt_enabler       body\n         prefix_proctype : ACTIVE opt_index proctypeprefix_proctype : proctypeopt_index : LBRACKET expr RBRACKET\n                     | LBRACKET NAME RBRACKET\n        opt_index : emptyinit : INIT opt_priority bodyclaim : CLAIM optname bodyutype : TYPEDEF NAME LBRACE decl_lst RBRACEltl : LTL LBRACE expr RBRACEdecl : decl_lstdecl : emptydecl_lst : one_decl SEMI decl_lstdecl_lst : one_declone_decl : vis typename var_list\n                    | vis NAME var_list\n        one_decl : typename var_list\n                    | NAME var_list\n        one_decl : vis MTYPE asgn LBRACE name_list RBRACEone_decl : MTYPE asgn LBRACE name_list RBRACEname_list : name_list COMMA NAMEname_list : NAMEvar_list : ivar COMMA var_listvar_list : ivarivar : vardclivar : vardcl asgn exprvardcl : NAMEvardcl : NAME COLON constvardcl : NAME LBRACKET const_expr RBRACKETvardcl : vardcl EQUALS ch_inittypename : BIT\n                    | BOOL\n                    | BYTE\n                    | CHAN\n                    | INT\n                    | PID\n                    | SHORT\n                    | UNSIGNED\n                    | MTYPE\n        ch_init : LBRACKET const_expr RBRACKET  OF LBRACE typ_list RBRACEtyp_list : typ_list COMMA basetypetyp_list : basetypebasetype : typenamevarref : cmpndcmpnd : cmpnd PERIOD cmpnd %prec DOTcmpnd : pfldpfld : NAME LBRACKET expr RBRACKETpfld : NAMEopt_priority : PRIORITY numberopt_priority : emptyopt_enabler : PROVIDED LPAREN expr RPARENopt_enabler : emptybody : LBRACE sequence os RBRACEsequence : sequence msemi stepsequence : seq_block stepsequence : stepseq_block : sequence msemi atomic\n                     | sequence msemi dstep\n        seq_block : seq_block atomic\n                     | seq_block dstep\n        seq_block : atomic\n                     | dstep\n        step : one_decl\n                | stmnt\n        step : NAME COLON one_declstep : NAME COLON XR\n                | NAME COLON XS\n        step : stmnt UNLESS stmntstmnt : special\n                 | statement\n        statement : varref asgn full_exprstatement : varref INCRstatement : varref DECRstatement : ASSERT full_exprstatement : varref RCV rargsstatement : varref RCV LT rargs GTstatement : varref R_RCV rargsstatement : varref R_RCV LT rargs GTstatement : varref TX2 margsstatement : full_exprstatement : ELSEstatement : atomicatomic : ATOMIC LBRACE sequence os RBRACEstatement : dstepdstep : D_STEP LBRACE sequence os RBRACEstatement : LBRACE sequence os RBRACEstatement : NAME LPAREN args RPARENstatement : varref asgn NAME LPAREN args RPAREN statementstatement : RETURN full_exprstatement : PRINT LPAREN STRING prargs RPARENspecial : varref RCVspecial : varref LNOT margsspecial : BREAKspecial : GOTO NAMEspecial : NAME COLON stmntspecial : NAME COLONspecial : IF options FIspecial : DO options ODoptions : optionoptions : options optionoption : COLONS sequence osfull_expr : expr\n                     | pexpr\n        pexpr : probe\n                 | LPAREN pexpr RPAREN\n                 | pexpr LAND pexpr\n                 | pexpr LAND expr\n                 | expr LAND pexpr\n                 | pexpr LOR pexpr\n                 | pexpr LOR expr\n                 | expr LOR pexpr\n        probe : FULL LPAREN varref RPAREN\n                 | NFULL LPAREN varref RPAREN\n                 | EMPTY LPAREN varref RPAREN\n                 | NEMPTY LPAREN varref RPAREN\n        expr : LPAREN expr RPARENexpr : expr PLUS expr\n                | expr MINUS expr\n                | expr TIMES expr\n                | expr DIVIDE expr\n                | expr MOD expr\n        expr : NOT expr\n                | MINUS expr %prec UMINUS\n                | LNOT expr %prec NEG\n        expr : expr AND expr\n                | expr OR expr\n                | expr XOR expr\n                | expr LAND expr\n                | expr LOR expr\n        expr : expr LSHIFT expr\n                | expr RSHIFT expr\n        expr : const\n                | varref\n        expr : varref RCV LBRACKET rargs RBRACKET\n                | varref R_RCV LBRACKET rargs RBRACKET\n        expr : LPAREN expr ARROW expr COLON expr RPAREN\n                | LEN LPAREN varref RPAREN\n                | ENABLED LPAREN expr RPAREN\n                | GET_P LPAREN expr RPAREN\n        expr : RUN aname LPAREN args RPAREN opt_priorityexpr : TIMEOUT\n                | NONPROGRESS\n                | PC_VAL LPAREN expr RPAREN\n        expr : NAME AT NAME\n        expr : NAME LBRACKET expr RBRACKET AT NAMEexpr : NAME LBRACKET expr RBRACKET COLON pfldexpr : expr EQ expr\n                | expr NE expr\n                | expr LT expr\n                | expr LE expr\n                | expr GT expr\n                | expr GE expr\n        expr : expr UNTIL expr\n                | expr WEAK_UNTIL expr\n                | expr RELEASE expr\n                | expr IMPLIES expr\n                | expr EQUIV expr\n        expr : NEXT expr\n                | ALWAYS expr\n                | EVENTUALLY expr\n        const_expr : constconst_expr : MINUS const_expr %prec UMINUSconst_expr : const_expr PLUS const_expr\n                      | const_expr MINUS const_expr\n                      | const_expr TIMES const_expr\n                      | const_expr DIVIDE const_expr\n                      | const_expr MOD const_expr\n        const_expr : LPAREN const_expr RPARENconst : boolean\n                 | number\n        boolean : TRUE\n                   | FALSE\n        number : INTEGERtwo_args : expr COMMA exprargs : argprargs : COMMA argprargs : emptyargs : emptymargs : arg\n                 | expr LPAREN arg RPAREN\n        arg : expr\n               | expr COMMA arg\n        rarg : varref\n                | EVAL LPAREN expr RPAREN\n        rargs : rarg\n                 | rarg COMMA rargs\n                 | rarg LPAREN rargs RPAREN\n                 | LPAREN rargs RPAREN\n        proctype : PROCTYPE\n                    | D_PROCTYPE\n        aname : NAMEoptname : NAMEoptname : emptyos : empty\n              | semi\n        msemi : semi\n                 | msemi semi\n        semi : SEMI\n                | ARROW\n        asgn : EQUALS\n                | empty\n        vis : HIDDEN\n               | SHOW\n               | ISLOCAL\n        empty : '
+_lr_signature = 'programrightEQUALSleftTX2RCVR_RCVleftIMPLIESEQUIVleftLORleftLANDleftALWAYSEVENTUALLYleftUNTILWEAK_UNTILRELEASErightNEXTleftORleftXORleftANDleftEQNEleftLTLEGTGEleftLSHIFTRSHIFTleftPLUSMINUSleftTIMESDIVIDEMODleftINCRDECRrightLNOTNOTUMINUSNEGleftDOTleftLPARENRPARENLBRACKETRBRACKETLPAREN RPAREN LBRACKET RBRACKET LBRACE RBRACE COMMA PERIOD SEMI COLONS COLON ELLIPSIS PLUS INCR MINUS DECR TIMES DIVIDE MOD OR AND NOT XOR IMPLIES EQUIV LOR LAND LNOT LT GT LE GE EQ NE RCV R_RCV TX2 LSHIFT RSHIFT AT ALWAYS EVENTUALLY EQUALS ARROW STRING NAME INTEGER PREPROC NEWLINE COMMENT ACTIVE ASSERT ATOMIC BIT BOOL BREAK BYTE CHAN CLAIM DO D_PROCTYPE D_STEP ELSE EMPTY ENABLED EVAL FALSE FI FULL GET_P GOTO HIDDEN IF INIT INT ISLOCAL LEN LTL MTYPE NEMPTY NEXT NFULL NONPROGRESS OD OF PC_VAL PID PRINT PRIORITY PROCTYPE PROVIDED RELEASE RETURN RUN SHORT SHOW TIMEOUT TRUE TYPEDEF UNLESS UNSIGNED UNTIL WEAK_UNTIL XR XSprogram : unitsunits : units unitunits : unitunit : proc\n                | init\n                | claim\n                | ltl\n        unit : one_decl\n                | utype\n        unit : semiproc : prefix_proctype NAME       LPAREN decl RPAREN       opt_priority opt_enabler       body\n         prefix_proctype : ACTIVE opt_index proctypeprefix_proctype : proctypeopt_index : LBRACKET expr RBRACKET\n                     | LBRACKET NAME RBRACKET\n        opt_index : emptyinit : INIT opt_priority bodyclaim : CLAIM optname bodyutype : TYPEDEF NAME LBRACE decl_lst RBRACEltl : LTL LBRACE expr RBRACEdecl : decl_lstdecl : emptydecl_lst : one_decl SEMI decl_lstdecl_lst : one_declone_decl : vis typename var_list\n                    | vis NAME var_list\n        one_decl : typename var_list\n                    | NAME var_list\n        one_decl : vis MTYPE asgn LBRACE name_list RBRACEone_decl : MTYPE asgn LBRACE name_list RBRACEname_list : name_list COMMA NAMEname_list : NAMEvar_list : ivar COMMA var_listvar_list : ivarivar : vardclivar : vardcl asgn exprvardcl : NAMEvardcl : NAME COLON constvardcl : NAME LBRACKET const_expr RBRACKETvardcl : vardcl EQUALS ch_inittypename : BIT\n                    | BOOL\n                    | BYTE\n                    | CHAN\n                    | INT\n                    | PID\n                    | SHORT\n                    | UNSIGNED\n                    | MTYPE\n        ch_init : LBRACKET const_expr RBRACKET  OF LBRACE typ_list RBRACEtyp_list : typ_list COMMA basetypetyp_list : basetypebasetype : typenamevarref : cmpndcmpnd : cmpnd PERIOD cmpnd %prec DOTcmpnd : pfldpfld : NAME LBRACKET expr RBRACKETpfld : NAMEopt_priority : PRIORITY numberopt_priority : emptyopt_enabler : PROVIDED LPAREN expr RPARENopt_enabler : emptybody : LBRACE sequence os RBRACEsequence : sequence msemi stepsequence : seq_block stepsequence : stepseq_block : sequence msemi atomic\n                     | sequence msemi dstep\n        seq_block : seq_block atomic\n                     | seq_block dstep\n        seq_block : atomic\n                     | dstep\n        step : one_decl\n                | stmnt\n        step : NAME COLON one_declstep : NAME COLON XR\n                | NAME COLON XS\n        step : stmnt UNLESS stmntstmnt : special\n                 | statement\n        statement : varref asgn full_exprstatement : varref INCRstatement : varref DECRstatement : ASSERT full_exprstatement : varref RCV rargsstatement : varref RCV LT rargs GTstatement : varref R_RCV rargsstatement : varref R_RCV LT rargs GTstatement : varref TX2 margsstatement : full_exprstatement : ELSEstatement : atomicatomic : ATOMIC LBRACE sequence os RBRACEstatement : dstepdstep : D_STEP LBRACE sequence os RBRACEstatement : LBRACE sequence os RBRACEstatement : NAME LPAREN args RPARENstatement : varref asgn NAME LPAREN args RPAREN statementstatement : RETURN full_exprstatement : PRINT LPAREN STRING prargs RPARENspecial : varref RCVspecial : varref LNOT margsspecial : BREAKspecial : GOTO NAMEspecial : NAME COLON stmntspecial : NAME COLONspecial : IF options FIspecial : DO options ODoptions : optionoptions : options optionoption : COLONS sequence osfull_expr : expr\n                     | pexpr\n        pexpr : probe\n                 | LPAREN pexpr RPAREN\n                 | pexpr LAND pexpr\n                 | pexpr LAND expr\n                 | expr LAND pexpr\n                 | pexpr LOR pexpr\n                 | pexpr LOR expr\n                 | expr LOR pexpr\n        probe : FULL LPAREN varref RPAREN\n                 | NFULL LPAREN varref RPAREN\n                 | EMPTY LPAREN varref RPAREN\n                 | NEMPTY LPAREN varref RPAREN\n        expr : LPAREN expr RPARENexpr : expr PLUS expr\n                | expr MINUS expr\n                | expr TIMES expr\n                | expr DIVIDE expr\n                | expr MOD expr\n        expr : NOT expr\n                | MINUS expr %prec UMINUS\n                | LNOT expr %prec NEG\n        expr : expr AND expr\n                | expr OR expr\n                | expr XOR expr\n                | expr LAND expr\n                | expr LOR expr\n        expr : expr LSHIFT expr\n                | expr RSHIFT expr\n        expr : const\n                | varref\n        expr : varref RCV LBRACKET rargs RBRACKET\n                | varref R_RCV LBRACKET rargs RBRACKET\n        expr : LPAREN expr ARROW expr COLON expr RPAREN\n                | LEN LPAREN varref RPAREN\n                | ENABLED LPAREN expr RPAREN\n                | GET_P LPAREN expr RPAREN\n        expr : RUN aname LPAREN args RPAREN opt_priorityexpr : TIMEOUT\n                | NONPROGRESS\n                | PC_VAL LPAREN expr RPAREN\n        expr : NAME AT NAME\n        expr : NAME LBRACKET expr RBRACKET AT NAMEexpr : NAME LBRACKET expr RBRACKET COLON pfldexpr : expr EQ expr\n                | expr NE expr\n                | expr LT expr\n                | expr LE expr\n                | expr GT expr\n                | expr GE expr\n        expr : expr UNTIL expr\n                | expr WEAK_UNTIL expr\n                | expr RELEASE expr\n                | expr IMPLIES expr\n                | expr EQUIV expr\n        expr : NEXT expr\n                | ALWAYS expr\n                | EVENTUALLY expr\n        const_expr : constconst_expr : MINUS const_expr %prec UMINUSconst_expr : const_expr PLUS const_expr\n                      | const_expr MINUS const_expr\n                      | const_expr TIMES const_expr\n                      | const_expr DIVIDE const_expr\n                      | const_expr MOD const_expr\n        const_expr : LPAREN const_expr RPARENconst : boolean\n                 | number\n        boolean : TRUE\n                   | FALSE\n        number : INTEGERtwo_args : expr COMMA exprargs : argprargs : COMMA argprargs : emptyargs : emptymargs : arg\n                 | expr LPAREN arg RPAREN\n        arg : expr\n               | expr COMMA arg\n        rarg : varref\n                | EVAL LPAREN expr RPAREN\n        rargs : rarg\n                 | rarg COMMA rargs\n                 | rarg LPAREN rargs RPAREN\n                 | LPAREN rargs RPAREN\n        proctype : PROCTYPE\n                    | D_PROCTYPE\n        aname : NAMEoptname : NAMEoptname : emptyos : empty\n              | semi\n        msemi : semi\n                 | msemi semi\n        semi : SEMI\n                | ARROW\n        asgn : EQUALS\n                | empty\n        vis : HIDDEN\n               | SHOW\n               | ISLOCAL\n        empty : '
     
 _lr_action_items = {'INIT':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[13,13,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'CLAIM':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[14,14,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'LTL':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[15,15,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'NAME':([0,2,3,4,5,6,7,8,9,10,11,12,14,16,17,18,19,20,21,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,39,40,41,42,45,49,50,51,52,53,55,56,59,61,64,65,66,67,68,69,70,71,73,74,75,76,77,78,82,83,84,86,87,88,89,90,91,92,93,94,95,96,97,99,100,101,108,113,114,115,117,120,121,122,125,130,132,136,138,139,148,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,173,174,175,178,179,180,183,184,185,186,187,188,189,190,197,198,209,211,213,214,215,216,217,218,219,220,221,222,225,226,230,237,238,239,240,241,242,243,244,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,269,270,271,273,276,278,280,282,283,284,295,297,298,299,301,304,317,319,327,341,351,352,353,354,356,357,358,365,367,371,372,374,375,376,380,382,383,389,390,391,393,394,395,396,397,400,401,415,416,417,418,427,428,430,432,433,436,],[12,12,-3,-4,-5,-6,-7,-8,-9,-10,38,39,47,51,39,-49,57,-208,-209,-13,-212,-213,-214,-41,-42,-43,-44,-45,-46,-47,-48,-199,-200,-2,-37,-28,-34,-35,-60,86,39,39,-49,-27,-210,-211,103,12,39,86,-210,-17,125,-59,-183,-18,86,86,86,86,-142,-143,182,-151,-152,-58,-56,86,86,86,-179,-180,-54,-181,-182,-25,-26,192,12,-12,-38,-33,-36,-40,125,125,-71,-72,39,-215,227,86,86,86,-20,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,86,-133,-132,-134,273,86,86,86,278,86,-168,-169,-170,273,192,12,-39,125,-206,-69,-70,301,304,86,125,125,273,86,325,273,86,125,86,86,86,86,273,273,273,273,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,86,273,273,-58,86,-154,-55,-30,359,-19,-63,-67,-68,-207,-58,39,273,273,273,86,-147,86,-148,-149,-153,-57,-29,301,86,273,273,86,86,86,86,86,86,86,-144,-145,-215,417,273,-11,86,-93,-95,-57,-150,-155,-156,433,-146,-50,-215,-58,273,]),'MTYPE':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[18,18,-3,-4,-5,-6,-7,-8,-9,-10,52,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,18,-17,18,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,18,-38,-33,-36,-40,18,18,-71,-72,-20,-133,-132,-134,-168,-169,-170,18,-39,18,-206,-69,-70,18,18,18,18,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,423,-93,-95,-57,-150,-155,-156,-146,-50,423,]),'TYPEDEF':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[19,19,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'SEMI':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,107,108,113,114,115,118,119,121,122,123,124,125,128,129,130,131,135,137,141,142,143,148,173,174,175,186,187,188,198,207,209,211,212,213,214,216,220,223,224,227,232,235,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,296,297,298,299,300,301,302,303,304,305,306,307,308,312,313,314,315,316,318,321,322,323,324,325,326,328,329,331,332,333,335,336,337,338,339,340,342,343,351,353,354,356,357,358,364,365,366,385,386,387,388,390,391,393,396,399,400,401,402,403,405,409,410,412,413,415,416,417,418,424,425,426,428,430,432,433,434,],[20,20,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,197,-38,-33,-36,-40,20,-66,-92,-94,-73,-74,-58,-79,-80,-143,-103,-90,-91,-112,-113,-114,-20,-133,-132,-134,-168,-169,-170,-39,20,20,-206,-65,-92,-94,-106,-101,-82,-83,-104,-84,-99,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-64,-92,-94,-207,-78,-58,-92,-94,-58,-75,-76,-77,-105,-191,20,20,-193,-85,-195,-102,-189,-191,-81,-58,-87,-89,-107,20,-108,-115,-138,-118,-139,-121,-116,-117,-119,-120,-147,-148,-149,-153,-57,-29,-96,-106,-97,-122,-123,-124,-125,-144,-145,-215,-11,-192,-93,-95,-86,-196,-198,-88,-100,-138,-139,-57,-150,-155,-156,-197,-194,-190,-146,-50,-143,-58,-98,]),'ARROW':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,118,119,121,122,123,124,125,128,129,130,131,135,137,141,142,143,148,172,173,174,175,186,187,188,198,207,209,211,212,213,214,216,220,223,224,227,232,233,235,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,296,297,298,299,300,301,302,303,304,305,306,307,308,312,313,314,315,316,318,321,322,323,324,325,326,328,329,331,332,333,335,336,337,338,339,340,342,343,351,353,354,356,357,358,364,365,366,384,385,386,387,388,390,391,393,396,399,400,401,402,403,405,409,410,412,413,415,416,417,418,424,425,426,428,430,432,433,434,],[21,21,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,21,-66,-92,-94,-73,-74,-58,-79,-80,-143,-103,-90,-91,-112,-113,-114,-20,269,-133,-132,-134,-168,-169,-170,-39,21,21,-206,-65,-92,-94,-106,-101,-82,-83,-104,-84,269,-99,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-64,-92,-94,-207,-78,-58,-92,-94,-58,-75,-76,-77,-105,-191,21,21,-193,-85,-195,-102,-189,-191,-81,-58,-87,-89,-107,21,-108,-115,-138,-118,-139,-121,-116,-117,-119,-120,-147,-148,-149,-153,-57,-29,-96,-106,-97,269,-122,-123,-124,-125,-144,-145,-215,-11,-192,-93,-95,-86,-196,-198,-88,-100,-138,-139,-57,-150,-155,-156,-197,-194,-190,-146,-50,-143,-58,-98,]),'ACTIVE':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[22,22,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'HIDDEN':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,400,401,415,416,417,418,428,430,],[24,24,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,24,-17,24,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,24,-38,-33,-36,-40,24,24,-71,-72,-20,-133,-132,-134,-168,-169,-170,24,-39,24,-206,-69,-70,24,24,24,24,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-93,-95,-57,-150,-155,-156,-146,-50,]),'SHOW':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,400,401,415,416,417,418,428,430,],[25,25,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,25,-17,25,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,25,-38,-33,-36,-40,25,25,-71,-72,-20,-133,-132,-134,-168,-169,-170,25,-39,25,-206,-69,-70,25,25,25,25,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-93,-95,-57,-150,-155,-156,-146,-50,]),'ISLOCAL':([0,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,400,401,415,416,417,418,428,430,],[26,26,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,26,-17,26,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,26,-38,-33,-36,-40,26,26,-71,-72,-20,-133,-132,-134,-168,-169,-170,26,-39,26,-206,-69,-70,26,26,26,26,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-93,-95,-57,-150,-155,-156,-146,-50,]),'BIT':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[27,27,-3,-4,-5,-6,-7,-8,-9,-10,27,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,27,-17,27,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,27,-38,-33,-36,-40,27,27,-71,-72,-20,-133,-132,-134,-168,-169,-170,27,-39,27,-206,-69,-70,27,27,27,27,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,27,-93,-95,-57,-150,-155,-156,-146,-50,27,]),'BOOL':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[28,28,-3,-4,-5,-6,-7,-8,-9,-10,28,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,28,-17,28,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,28,-38,-33,-36,-40,28,28,-71,-72,-20,-133,-132,-134,-168,-169,-170,28,-39,28,-206,-69,-70,28,28,28,28,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,28,-93,-95,-57,-150,-155,-156,-146,-50,28,]),'BYTE':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[29,29,-3,-4,-5,-6,-7,-8,-9,-10,29,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,29,-17,29,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,29,-38,-33,-36,-40,29,29,-71,-72,-20,-133,-132,-134,-168,-169,-170,29,-39,29,-206,-69,-70,29,29,29,29,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,29,-93,-95,-57,-150,-155,-156,-146,-50,29,]),'CHAN':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[30,30,-3,-4,-5,-6,-7,-8,-9,-10,30,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,30,-17,30,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,30,-38,-33,-36,-40,30,30,-71,-72,-20,-133,-132,-134,-168,-169,-170,30,-39,30,-206,-69,-70,30,30,30,30,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,30,-93,-95,-57,-150,-155,-156,-146,-50,30,]),'INT':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[31,31,-3,-4,-5,-6,-7,-8,-9,-10,31,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,31,-17,31,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,31,-38,-33,-36,-40,31,31,-71,-72,-20,-133,-132,-134,-168,-169,-170,31,-39,31,-206,-69,-70,31,31,31,31,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,31,-93,-95,-57,-150,-155,-156,-146,-50,31,]),'PID':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[32,32,-3,-4,-5,-6,-7,-8,-9,-10,32,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,32,-17,32,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,32,-38,-33,-36,-40,32,32,-71,-72,-20,-133,-132,-134,-168,-169,-170,32,-39,32,-206,-69,-70,32,32,32,32,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,32,-93,-95,-57,-150,-155,-156,-146,-50,32,]),'SHORT':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[33,33,-3,-4,-5,-6,-7,-8,-9,-10,33,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,33,-17,33,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,33,-38,-33,-36,-40,33,33,-71,-72,-20,-133,-132,-134,-168,-169,-170,33,-39,33,-206,-69,-70,33,33,33,33,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,33,-93,-95,-57,-150,-155,-156,-146,-50,33,]),'UNSIGNED':([0,2,3,4,5,6,7,8,9,10,16,20,21,24,25,26,37,39,40,41,42,45,53,61,67,68,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,100,108,113,114,115,117,120,121,122,148,173,174,175,186,187,188,197,198,209,211,213,214,216,218,219,230,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,297,298,299,351,353,354,356,357,358,390,391,393,396,398,400,401,415,416,417,418,428,430,431,],[34,34,-3,-4,-5,-6,-7,-8,-9,-10,34,-208,-209,-212,-213,-214,-2,-37,-28,-34,-35,-60,-27,34,-17,34,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,34,-38,-33,-36,-40,34,34,-71,-72,-20,-133,-132,-134,-168,-169,-170,34,-39,34,-206,-69,-70,34,34,34,34,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-67,-68,-207,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,34,-93,-95,-57,-150,-155,-156,-146,-50,34,]),'PROCTYPE':([0,2,3,4,5,6,7,8,9,10,20,21,22,37,39,40,41,42,45,53,58,60,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,194,195,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[35,35,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-215,-2,-37,-28,-34,-35,-60,-27,35,-16,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-14,-15,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'D_PROCTYPE':([0,2,3,4,5,6,7,8,9,10,20,21,22,37,39,40,41,42,45,53,58,60,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,194,195,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[36,36,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-215,-2,-37,-28,-34,-35,-60,-27,36,-16,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-14,-15,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'$end':([1,2,3,4,5,6,7,8,9,10,20,21,37,39,40,41,42,45,53,67,69,70,71,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,148,173,174,175,186,187,188,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,284,295,351,353,354,356,357,358,390,391,393,396,415,416,417,418,428,430,],[0,-1,-3,-4,-5,-6,-7,-8,-9,-10,-208,-209,-2,-37,-28,-34,-35,-60,-27,-17,-59,-183,-18,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-20,-133,-132,-134,-168,-169,-170,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-19,-63,-147,-148,-149,-153,-57,-29,-144,-145,-215,-11,-57,-150,-155,-156,-146,-50,]),'PRIORITY':([13,196,393,],[44,44,44,]),'LBRACE':([13,14,15,18,20,21,43,45,46,47,48,52,54,55,56,57,68,69,70,98,117,120,121,122,126,127,196,209,211,213,214,215,216,218,219,230,285,297,298,299,360,362,363,365,400,401,427,429,],[-215,-215,49,-215,-208,-209,68,-60,68,-202,-203,-215,99,-210,-211,100,117,-59,-183,190,117,117,-71,-72,218,219,-215,117,-206,-69,-70,117,117,117,117,117,-215,-67,-68,-207,68,-62,398,117,-93,-95,117,-61,]),'EQUALS':([18,39,42,52,70,87,91,92,93,94,95,108,115,125,130,198,273,280,301,304,357,415,430,432,433,],[55,-37,66,55,-183,-56,-179,-180,-54,-181,-182,-38,-40,-58,55,-39,-58,-55,-58,-58,-57,-57,-50,55,-58,]),'RBRACE':([20,21,27,28,29,30,31,32,33,34,39,40,41,42,45,53,69,70,72,77,78,83,84,86,87,91,92,93,94,95,96,97,107,108,113,114,115,118,119,121,122,123,124,125,128,129,130,131,135,137,141,142,143,173,174,175,186,187,188,191,192,193,198,207,208,210,211,212,213,214,216,220,223,224,227,232,235,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,281,282,286,294,296,297,298,300,301,302,303,304,305,306,307,308,312,313,314,315,316,318,321,322,323,324,325,326,328,329,332,333,335,336,337,338,339,340,342,343,351,353,354,356,357,358,359,364,365,366,368,369,385,386,387,388,390,391,393,399,400,401,402,403,405,409,410,412,413,415,416,417,418,420,421,422,423,424,425,426,428,430,432,433,434,435,],[-208,-209,-41,-42,-43,-44,-45,-46,-47,-48,-37,-28,-34,-35,-60,-27,-59,-183,148,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-24,-38,-33,-36,-40,-215,-66,-92,-94,-73,-74,-58,-79,-80,-143,-103,-90,-91,-112,-113,-114,-133,-132,-134,-168,-169,-170,282,-32,284,-39,-215,295,-204,-205,-65,-92,-94,-106,-101,-82,-83,-104,-84,-99,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,358,-30,-23,364,-64,-92,-94,-78,-58,-92,-94,-58,-75,-76,-77,-105,-191,-215,-215,-193,-85,-195,-102,-189,-191,-81,-58,-87,-89,-107,-108,-115,-138,-118,-139,-121,-116,-117,-119,-120,-147,-148,-149,-153,-57,-29,-31,-96,-106,-97,400,401,-122,-123,-124,-125,-144,-145,-215,-192,-93,-95,-86,-196,-198,-88,-100,-138,-139,-57,-150,-155,-156,430,-52,-53,-49,-197,-194,-190,-146,-50,-143,-58,-98,-51,]),'ATOMIC':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,427,],[-208,-209,126,126,126,-71,-72,126,-206,-69,-70,126,126,126,126,126,-67,-68,-207,126,-93,-95,126,]),'D_STEP':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,427,],[-208,-209,127,127,127,-71,-72,127,-206,-69,-70,127,127,127,127,127,-67,-68,-207,127,-93,-95,127,]),'BREAK':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,],[-208,-209,131,131,131,-71,-72,131,-206,-69,-70,131,131,131,131,131,-67,-68,-207,131,-93,-95,]),'GOTO':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,],[-208,-209,132,132,132,-71,-72,132,-206,-69,-70,132,132,132,132,132,-67,-68,-207,132,-93,-95,]),'IF':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,],[-208,-209,133,133,133,-71,-72,133,-206,-69,-70,133,133,133,133,133,-67,-68,-207,133,-93,-95,]),'DO':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,],[-208,-209,134,134,134,-71,-72,134,-206,-69,-70,134,134,134,134,134,-67,-68,-207,134,-93,-95,]),'ASSERT':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,427,],[-208,-209,136,136,136,-71,-72,136,-206,-69,-70,136,136,136,136,136,-67,-68,-207,136,-93,-95,136,]),'ELSE':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,427,],[-208,-209,137,137,137,-71,-72,137,-206,-69,-70,137,137,137,137,137,-67,-68,-207,137,-93,-95,137,]),'RETURN':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,427,],[-208,-209,139,139,139,-71,-72,139,-206,-69,-70,139,139,139,139,139,-67,-68,-207,139,-93,-95,139,]),'PRINT':([20,21,68,117,120,121,122,209,211,213,214,215,216,218,219,230,297,298,299,365,400,401,427,],[-208,-209,140,140,140,-71,-72,140,-206,-69,-70,140,140,140,140,140,-67,-68,-207,140,-93,-95,140,]),'LPAREN':([20,21,38,39,42,45,49,55,56,59,63,65,66,68,69,70,73,74,75,76,77,78,79,80,81,83,84,85,86,87,88,89,90,91,92,93,94,95,108,111,112,115,116,117,120,121,122,125,130,136,138,139,140,144,145,146,147,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,173,174,175,179,180,181,182,183,185,186,187,188,198,199,200,201,202,203,209,211,213,214,215,216,217,218,219,220,221,222,225,226,230,237,238,239,240,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,269,270,271,273,276,278,280,297,298,299,301,304,315,317,318,319,320,323,325,327,341,351,352,353,354,356,357,361,365,367,371,372,374,375,376,380,382,383,389,390,391,393,397,400,401,415,416,417,418,425,427,428,430,432,433,436,],[-208,-209,61,-37,-215,-60,73,-210,-211,73,112,73,-210,138,-59,-183,73,73,73,73,-142,-143,178,179,180,-151,-152,183,-58,-56,73,73,73,-179,-180,-54,-181,-182,-38,112,112,-40,112,138,138,-71,-72,217,-215,138,138,138,236,241,242,243,244,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,73,-133,-132,-134,73,73,276,-201,73,73,-168,-169,-170,-39,112,112,112,112,112,138,-206,-69,-70,138,138,73,138,138,319,73,138,319,73,138,138,138,341,341,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,73,319,319,-58,73,-154,-55,-67,-68,-207,217,217,-193,319,372,319,374,375,376,319,341,-147,73,-148,-149,-153,-57,397,138,73,319,319,73,73,73,73,341,341,73,-144,-145,-215,73,-93,-95,-57,-150,-155,-156,-194,138,-146,-50,-215,217,319,]),'NOT':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,75,-210,-211,75,75,-210,75,-183,75,75,75,75,-56,75,75,75,-179,-180,-54,-181,-182,-38,-40,75,75,-71,-72,-58,-215,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,75,-39,75,-206,-69,-70,75,75,75,75,75,75,75,75,75,75,75,75,75,75,-58,75,-55,-67,-68,-207,-58,-58,75,75,-57,75,75,75,75,75,75,75,75,75,75,-93,-95,-57,75,-50,-215,-58,]),'MINUS':([20,21,39,42,45,49,55,56,59,63,65,66,68,69,70,72,73,74,75,76,77,78,83,84,86,87,88,89,90,91,92,93,94,95,102,103,108,109,110,111,112,114,115,116,117,120,121,122,125,130,136,138,139,141,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,172,173,174,175,179,180,183,185,186,187,188,198,199,200,201,202,203,204,205,206,209,211,213,214,215,216,217,218,219,221,222,226,230,233,237,238,239,240,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,269,273,274,275,276,277,278,279,280,287,288,289,290,291,292,297,298,299,301,304,312,323,325,335,337,340,341,343,348,351,352,353,354,356,357,365,367,374,375,376,380,382,383,384,389,390,391,392,393,397,400,401,406,412,413,414,415,416,417,418,419,427,428,430,432,433,],[-208,-209,-37,-215,-60,74,-210,-211,74,111,74,-210,74,-59,-183,150,74,74,74,74,-142,-143,-151,-152,-58,-56,74,74,74,-179,-180,-54,-181,-182,150,-58,-38,200,-171,111,111,150,-40,111,74,74,-71,-72,-58,-143,74,74,74,150,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,74,150,-133,-132,-134,74,74,74,74,150,150,150,-39,111,111,111,111,111,-172,200,200,74,-206,-69,-70,74,74,74,74,74,74,74,74,74,150,74,74,74,74,-127,-128,-129,-130,-131,150,150,150,150,150,150,150,150,150,150,150,150,150,150,150,150,150,150,-126,74,-58,150,150,74,150,-154,150,-55,-173,-174,-175,-176,-177,-178,-67,-68,-207,-58,-58,150,150,-58,150,150,150,74,150,150,-147,74,-148,-149,-153,-57,74,74,74,74,74,74,74,74,150,74,-144,-145,150,-215,74,-93,-95,150,150,150,150,-57,-150,-155,-156,150,74,-146,-50,-143,-58,]),'LNOT':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,76,-210,-211,76,76,-210,76,-183,76,76,76,76,-56,76,76,76,-179,-180,-54,-181,-182,-38,-40,76,76,-71,-72,-58,221,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,76,-39,76,-206,-69,-70,76,76,76,76,76,76,76,76,76,76,76,76,76,76,-58,76,-55,-67,-68,-207,-58,-58,76,76,-57,76,76,76,76,76,76,76,76,76,76,-93,-95,-57,76,-50,-215,-58,]),'LEN':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,79,-210,-211,79,79,-210,79,-183,79,79,79,79,-56,79,79,79,-179,-180,-54,-181,-182,-38,-40,79,79,-71,-72,-58,-215,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,79,-39,79,-206,-69,-70,79,79,79,79,79,79,79,79,79,79,79,79,79,79,-58,79,-55,-67,-68,-207,-58,-58,79,79,-57,79,79,79,79,79,79,79,79,79,79,-93,-95,-57,79,-50,-215,-58,]),'ENABLED':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,80,-210,-211,80,80,-210,80,-183,80,80,80,80,-56,80,80,80,-179,-180,-54,-181,-182,-38,-40,80,80,-71,-72,-58,-215,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,80,-39,80,-206,-69,-70,80,80,80,80,80,80,80,80,80,80,80,80,80,80,-58,80,-55,-67,-68,-207,-58,-58,80,80,-57,80,80,80,80,80,80,80,80,80,80,-93,-95,-57,80,-50,-215,-58,]),'GET_P':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,81,-210,-211,81,81,-210,81,-183,81,81,81,81,-56,81,81,81,-179,-180,-54,-181,-182,-38,-40,81,81,-71,-72,-58,-215,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,81,-39,81,-206,-69,-70,81,81,81,81,81,81,81,81,81,81,81,81,81,81,-58,81,-55,-67,-68,-207,-58,-58,81,81,-57,81,81,81,81,81,81,81,81,81,81,-93,-95,-57,81,-50,-215,-58,]),'RUN':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,82,-210,-211,82,82,-210,82,-183,82,82,82,82,-56,82,82,82,-179,-180,-54,-181,-182,-38,-40,82,82,-71,-72,-58,-215,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,82,-39,82,-206,-69,-70,82,82,82,82,82,82,82,82,82,82,82,82,82,82,-58,82,-55,-67,-68,-207,-58,-58,82,82,-57,82,82,82,82,82,82,82,82,82,82,-93,-95,-57,82,-50,-215,-58,]),'TIMEOUT':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,83,-210,-211,83,83,-210,83,-183,83,83,83,83,-56,83,83,83,-179,-180,-54,-181,-182,-38,-40,83,83,-71,-72,-58,-215,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,83,-39,83,-206,-69,-70,83,83,83,83,83,83,83,83,83,83,83,83,83,83,-58,83,-55,-67,-68,-207,-58,-58,83,83,-57,83,83,83,83,83,83,83,83,83,83,-93,-95,-57,83,-50,-215,-58,]),'NONPROGRESS':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,84,-210,-211,84,84,-210,84,-183,84,84,84,84,-56,84,84,84,-179,-180,-54,-181,-182,-38,-40,84,84,-71,-72,-58,-215,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,84,-39,84,-206,-69,-70,84,84,84,84,84,84,84,84,84,84,84,84,84,84,-58,84,-55,-67,-68,-207,-58,-58,84,84,-57,84,84,84,84,84,84,84,84,84,84,-93,-95,-57,84,-50,-215,-58,]),'PC_VAL':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,85,-210,-211,85,85,-210,85,-183,85,85,85,85,-56,85,85,85,-179,-180,-54,-181,-182,-38,-40,85,85,-71,-72,-58,-215,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,85,-39,85,-206,-69,-70,85,85,85,85,85,85,85,85,85,85,85,85,85,85,-58,85,-55,-67,-68,-207,-58,-58,85,85,-57,85,85,85,85,85,85,85,85,85,85,-93,-95,-57,85,-50,-215,-58,]),'NEXT':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,88,-210,-211,88,88,-210,88,-183,88,88,88,88,-56,88,88,88,-179,-180,-54,-181,-182,-38,-40,88,88,-71,-72,-58,-215,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,88,-39,88,-206,-69,-70,88,88,88,88,88,88,88,88,88,88,88,88,88,88,-58,88,-55,-67,-68,-207,-58,-58,88,88,-57,88,88,88,88,88,88,88,88,88,88,-93,-95,-57,88,-50,-215,-58,]),'ALWAYS':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,89,-210,-211,89,89,-210,89,-183,89,89,89,89,-56,89,89,89,-179,-180,-54,-181,-182,-38,-40,89,89,-71,-72,-58,-215,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,89,-39,89,-206,-69,-70,89,89,89,89,89,89,89,89,89,89,89,89,89,89,-58,89,-55,-67,-68,-207,-58,-58,89,89,-57,89,89,89,89,89,89,89,89,89,89,-93,-95,-57,89,-50,-215,-58,]),'EVENTUALLY':([20,21,39,42,49,55,56,59,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,115,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,90,-210,-211,90,90,-210,90,-183,90,90,90,90,-56,90,90,90,-179,-180,-54,-181,-182,-38,-40,90,90,-71,-72,-58,-215,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,90,-39,90,-206,-69,-70,90,90,90,90,90,90,90,90,90,90,90,90,90,90,-58,90,-55,-67,-68,-207,-58,-58,90,90,-57,90,90,90,90,90,90,90,90,90,90,-93,-95,-57,90,-50,-215,-58,]),'FULL':([20,21,55,56,68,87,93,117,120,121,122,125,130,136,138,139,209,211,213,214,215,216,218,219,222,230,237,238,239,240,273,280,297,298,299,301,304,341,357,365,382,383,400,401,415,427,432,433,],[-208,-209,-210,-211,144,-56,-54,144,144,-71,-72,-58,-215,144,144,144,144,-206,-69,-70,144,144,144,144,144,144,144,144,144,144,-58,-55,-67,-68,-207,-58,-58,144,-57,144,144,144,-93,-95,-57,144,-215,-58,]),'NFULL':([20,21,55,56,68,87,93,117,120,121,122,125,130,136,138,139,209,211,213,214,215,216,218,219,222,230,237,238,239,240,273,280,297,298,299,301,304,341,357,365,382,383,400,401,415,427,432,433,],[-208,-209,-210,-211,145,-56,-54,145,145,-71,-72,-58,-215,145,145,145,145,-206,-69,-70,145,145,145,145,145,145,145,145,145,145,-58,-55,-67,-68,-207,-58,-58,145,-57,145,145,145,-93,-95,-57,145,-215,-58,]),'EMPTY':([20,21,55,56,68,87,93,117,120,121,122,125,130,136,138,139,209,211,213,214,215,216,218,219,222,230,237,238,239,240,273,280,297,298,299,301,304,341,357,365,382,383,400,401,415,427,432,433,],[-208,-209,-210,-211,146,-56,-54,146,146,-71,-72,-58,-215,146,146,146,146,-206,-69,-70,146,146,146,146,146,146,146,146,146,146,-58,-55,-67,-68,-207,-58,-58,146,-57,146,146,146,-93,-95,-57,146,-215,-58,]),'NEMPTY':([20,21,55,56,68,87,93,117,120,121,122,125,130,136,138,139,209,211,213,214,215,216,218,219,222,230,237,238,239,240,273,280,297,298,299,301,304,341,357,365,382,383,400,401,415,427,432,433,],[-208,-209,-210,-211,147,-56,-54,147,147,-71,-72,-58,-215,147,147,147,147,-206,-69,-70,147,147,147,147,147,147,147,147,147,147,-58,-55,-67,-68,-207,-58,-58,147,-57,147,147,147,-93,-95,-57,147,-215,-58,]),'TRUE':([20,21,39,42,49,55,56,59,62,63,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,111,112,115,116,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,199,200,201,202,203,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,94,-210,-211,94,94,94,94,-210,94,-183,94,94,94,94,-56,94,94,94,-179,-180,-54,-181,-182,-38,94,94,-40,94,94,94,-71,-72,-58,-215,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,94,-39,94,94,94,94,94,94,-206,-69,-70,94,94,94,94,94,94,94,94,94,94,94,94,94,94,-58,94,-55,-67,-68,-207,-58,-58,94,94,-57,94,94,94,94,94,94,94,94,94,94,-93,-95,-57,94,-50,-215,-58,]),'FALSE':([20,21,39,42,49,55,56,59,62,63,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,111,112,115,116,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,199,200,201,202,203,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,95,-210,-211,95,95,95,95,-210,95,-183,95,95,95,95,-56,95,95,95,-179,-180,-54,-181,-182,-38,95,95,-40,95,95,95,-71,-72,-58,-215,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,95,-39,95,95,95,95,95,95,-206,-69,-70,95,95,95,95,95,95,95,95,95,95,95,95,95,95,-58,95,-55,-67,-68,-207,-58,-58,95,95,-57,95,95,95,95,95,95,95,95,95,95,-93,-95,-57,95,-50,-215,-58,]),'INTEGER':([20,21,39,42,44,49,55,56,59,62,63,65,66,68,70,73,74,75,76,87,88,89,90,91,92,93,94,95,108,111,112,115,116,117,120,121,122,125,130,136,138,139,149,150,151,152,153,154,155,156,157,158,159,160,161,162,163,164,165,166,167,168,169,170,171,179,180,183,185,198,199,200,201,202,203,209,211,213,214,215,216,217,218,219,221,222,226,230,237,238,239,240,269,273,276,280,297,298,299,301,304,341,352,357,365,367,374,375,376,380,382,383,389,397,400,401,415,427,430,432,433,],[-208,-209,-37,-215,70,70,-210,-211,70,70,70,70,-210,70,-183,70,70,70,70,-56,70,70,70,-179,-180,-54,-181,-182,-38,70,70,-40,70,70,70,-71,-72,-58,-215,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,-39,70,70,70,70,70,70,-206,-69,-70,70,70,70,70,70,70,70,70,70,70,70,70,70,70,-58,70,-55,-67,-68,-207,-58,-58,70,70,-57,70,70,70,70,70,70,70,70,70,70,-93,-95,-57,70,-50,-215,-58,]),'FI':([20,21,39,40,41,42,45,53,69,70,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,119,121,122,123,124,125,128,129,130,131,135,137,141,142,143,173,174,175,186,187,188,198,210,211,212,213,214,216,220,223,224,227,228,229,232,235,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,296,297,298,300,301,302,303,304,305,306,307,308,312,315,316,318,321,322,323,324,325,326,328,329,330,331,332,333,335,336,337,338,339,340,342,343,351,353,354,356,357,358,364,365,366,378,385,386,387,388,390,391,393,399,400,401,402,403,405,409,410,412,413,415,416,417,418,424,425,426,428,430,432,433,434,],[-208,-209,-37,-28,-34,-35,-60,-27,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-66,-92,-94,-73,-74,-58,-79,-80,-143,-103,-90,-91,-112,-113,-114,-133,-132,-134,-168,-169,-170,-39,-204,-205,-65,-92,-94,-106,-101,-82,-83,-104,329,-109,-84,-99,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-64,-92,-94,-78,-58,-92,-94,-58,-75,-76,-77,-105,-191,-193,-85,-195,-102,-189,-191,-81,-58,-87,-89,-107,-110,-215,-108,-115,-138,-118,-139,-121,-116,-117,-119,-120,-147,-148,-149,-153,-57,-29,-96,-106,-97,-111,-122,-123,-124,-125,-144,-145,-215,-192,-93,-95,-86,-196,-198,-88,-100,-138,-139,-57,-150,-155,-156,-197,-194,-190,-146,-50,-143,-58,-98,]),'COLONS':([20,21,39,40,41,42,45,53,69,70,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,119,121,122,123,124,125,128,129,130,131,133,134,135,137,141,142,143,173,174,175,186,187,188,198,210,211,212,213,214,216,220,223,224,227,228,229,231,232,235,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,296,297,298,300,301,302,303,304,305,306,307,308,312,315,316,318,321,322,323,324,325,326,328,329,330,331,332,333,335,336,337,338,339,340,342,343,351,353,354,356,357,358,364,365,366,378,385,386,387,388,390,391,393,399,400,401,402,403,405,409,410,412,413,415,416,417,418,424,425,426,428,430,432,433,434,],[-208,-209,-37,-28,-34,-35,-60,-27,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-66,-92,-94,-73,-74,-58,-79,-80,-143,-103,230,230,-90,-91,-112,-113,-114,-133,-132,-134,-168,-169,-170,-39,-204,-205,-65,-92,-94,-106,-101,-82,-83,-104,230,-109,230,-84,-99,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-64,-92,-94,-78,-58,-92,-94,-58,-75,-76,-77,-105,-191,-193,-85,-195,-102,-189,-191,-81,-58,-87,-89,-107,-110,-215,-108,-115,-138,-118,-139,-121,-116,-117,-119,-120,-147,-148,-149,-153,-57,-29,-96,-106,-97,-111,-122,-123,-124,-125,-144,-145,-215,-192,-93,-95,-86,-196,-198,-88,-100,-138,-139,-57,-150,-155,-156,-197,-194,-190,-146,-50,-143,-58,-98,]),'OD':([20,21,39,40,41,42,45,53,69,70,77,78,83,84,86,87,91,92,93,94,95,96,97,108,113,114,115,119,121,122,123,124,125,128,129,130,131,135,137,141,142,143,173,174,175,186,187,188,198,210,211,212,213,214,216,220,223,224,227,229,231,232,235,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,282,296,297,298,300,301,302,303,304,305,306,307,308,312,315,316,318,321,322,323,324,325,326,328,329,330,331,332,333,335,336,337,338,339,340,342,343,351,353,354,356,357,358,364,365,366,378,385,386,387,388,390,391,393,399,400,401,402,403,405,409,410,412,413,415,416,417,418,424,425,426,428,430,432,433,434,],[-208,-209,-37,-28,-34,-35,-60,-27,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,-38,-33,-36,-40,-66,-92,-94,-73,-74,-58,-79,-80,-143,-103,-90,-91,-112,-113,-114,-133,-132,-134,-168,-169,-170,-39,-204,-205,-65,-92,-94,-106,-101,-82,-83,-104,-109,332,-84,-99,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-30,-64,-92,-94,-78,-58,-92,-94,-58,-75,-76,-77,-105,-191,-193,-85,-195,-102,-189,-191,-81,-58,-87,-89,-107,-110,-215,-108,-115,-138,-118,-139,-121,-116,-117,-119,-120,-147,-148,-149,-153,-57,-29,-96,-106,-97,-111,-122,-123,-124,-125,-144,-145,-215,-192,-93,-95,-86,-196,-198,-88,-100,-138,-139,-57,-150,-155,-156,-197,-194,-190,-146,-50,-143,-58,-98,]),'LBRACKET':([22,39,66,86,103,125,176,177,220,225,273,301,304,325,433,436,],[59,63,116,185,185,185,270,271,270,271,352,185,185,185,185,270,]),'COMMA':([27,28,29,30,31,32,33,34,39,41,42,45,69,70,77,78,83,84,86,87,91,92,93,94,95,108,114,115,173,174,175,186,187,188,191,192,198,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,281,312,315,318,323,334,351,353,354,356,357,359,390,391,393,415,416,417,418,420,421,422,423,425,428,430,435,],[-41,-42,-43,-44,-45,-46,-47,-48,-37,64,-35,-60,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-38,-36,-40,-133,-132,-134,-168,-169,-170,283,-32,-39,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,283,367,-193,371,367,380,-147,-148,-149,-153,-57,-31,-144,-145,-215,-57,-150,-155,-156,431,-52,-53,-49,-194,-146,-50,-51,]),'RPAREN':([39,40,41,42,45,53,61,69,70,77,78,83,84,86,87,91,92,93,94,95,96,97,104,105,106,107,108,110,113,114,115,143,172,173,174,175,186,187,188,198,204,205,217,233,234,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,272,273,274,275,276,277,278,280,282,286,287,288,289,290,291,292,309,310,311,312,315,318,333,334,335,336,337,338,339,340,342,343,344,345,346,347,351,353,354,355,356,357,358,373,376,379,381,384,385,386,387,388,390,391,393,399,403,404,405,406,407,408,411,412,413,414,415,416,417,418,419,424,425,428,430,],[-37,-28,-34,-35,-60,-27,-215,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-25,-26,196,-21,-22,-24,-38,-171,-33,-36,-40,-114,268,-133,-132,-134,-168,-169,-170,-39,-172,292,-215,268,333,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,351,-58,353,354,-215,356,-154,-55,-30,-23,-173,-174,-175,-176,-177,-178,366,-185,-188,-191,-193,-195,-115,-215,-138,-118,-139,-121,-116,-117,-119,-120,385,386,387,388,-147,-148,-149,393,-153,-57,-29,405,-215,410,-187,268,-122,-123,-124,-125,-144,-145,-215,-192,-196,424,-198,425,426,427,-186,-138,-139,428,-57,-150,-155,-156,429,-197,-194,-146,-50,]),'COLON':([39,45,69,70,77,78,83,84,86,87,91,92,93,94,95,125,173,174,175,186,187,188,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,301,304,348,351,353,354,356,357,390,391,393,415,416,417,418,428,],[62,-60,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,216,-133,-132,-134,-168,-169,-170,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,365,365,389,-147,-148,-149,-153,-57,-144,-145,-215,-57,-150,-155,-156,-146,]),'PROVIDED':([45,69,70,196,285,],[-60,-59,-183,-215,361,]),'PLUS':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,109,110,114,125,130,141,172,173,174,175,186,187,188,204,205,206,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,287,288,289,290,291,292,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,149,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,149,-58,199,-171,149,-58,-143,149,149,-133,-132,-134,149,149,149,-172,199,199,149,-127,-128,-129,-130,-131,149,149,149,149,149,149,149,149,149,149,149,149,149,149,149,149,149,149,-126,-58,149,149,149,-154,149,-55,-173,-174,-175,-176,-177,-178,-58,-58,149,149,-58,149,149,149,149,149,-147,-148,-149,-153,-57,149,-144,-145,149,-215,149,149,149,149,-57,-150,-155,-156,149,-146,-143,-58,]),'TIMES':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,109,110,114,125,130,141,172,173,174,175,186,187,188,204,205,206,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,287,288,289,290,291,292,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,151,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,151,-58,201,-171,151,-58,-143,151,151,-133,-132,-134,151,151,151,-172,201,201,151,151,151,-129,-130,-131,151,151,151,151,151,151,151,151,151,151,151,151,151,151,151,151,151,151,-126,-58,151,151,151,-154,151,-55,201,201,-175,-176,-177,-178,-58,-58,151,151,-58,151,151,151,151,151,-147,-148,-149,-153,-57,151,-144,-145,151,-215,151,151,151,151,-57,-150,-155,-156,151,-146,-143,-58,]),'DIVIDE':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,109,110,114,125,130,141,172,173,174,175,186,187,188,204,205,206,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,287,288,289,290,291,292,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,152,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,152,-58,202,-171,152,-58,-143,152,152,-133,-132,-134,152,152,152,-172,202,202,152,152,152,-129,-130,-131,152,152,152,152,152,152,152,152,152,152,152,152,152,152,152,152,152,152,-126,-58,152,152,152,-154,152,-55,202,202,-175,-176,-177,-178,-58,-58,152,152,-58,152,152,152,152,152,-147,-148,-149,-153,-57,152,-144,-145,152,-215,152,152,152,152,-57,-150,-155,-156,152,-146,-143,-58,]),'MOD':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,109,110,114,125,130,141,172,173,174,175,186,187,188,204,205,206,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,287,288,289,290,291,292,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,153,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,153,-58,203,-171,153,-58,-143,153,153,-133,-132,-134,153,153,153,-172,203,203,153,153,153,-129,-130,-131,153,153,153,153,153,153,153,153,153,153,153,153,153,153,153,153,153,153,-126,-58,153,153,153,-154,153,-55,203,203,-175,-176,-177,-178,-58,-58,153,153,-58,153,153,153,153,153,-147,-148,-149,-153,-57,153,-144,-145,153,-215,153,153,153,153,-57,-150,-155,-156,153,-146,-143,-58,]),'AND':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,154,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,154,-58,154,-58,-143,154,154,-133,-132,-134,154,154,154,154,-127,-128,-129,-130,-131,-135,154,154,154,154,-140,-141,-157,-158,-159,-160,-161,-162,154,154,154,154,154,-126,-58,154,154,154,-154,154,-55,-58,-58,154,154,-58,154,154,154,154,154,-147,-148,-149,-153,-57,154,-144,-145,154,-215,154,154,154,154,-57,-150,-155,-156,154,-146,-143,-58,]),'OR':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,155,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,155,-58,155,-58,-143,155,155,-133,-132,-134,155,155,155,155,-127,-128,-129,-130,-131,-135,-136,-137,155,155,-140,-141,-157,-158,-159,-160,-161,-162,155,155,155,155,155,-126,-58,155,155,155,-154,155,-55,-58,-58,155,155,-58,155,155,155,155,155,-147,-148,-149,-153,-57,155,-144,-145,155,-215,155,155,155,155,-57,-150,-155,-156,155,-146,-143,-58,]),'XOR':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,156,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,156,-58,156,-58,-143,156,156,-133,-132,-134,156,156,156,156,-127,-128,-129,-130,-131,-135,156,-137,156,156,-140,-141,-157,-158,-159,-160,-161,-162,156,156,156,156,156,-126,-58,156,156,156,-154,156,-55,-58,-58,156,156,-58,156,156,156,156,156,-147,-148,-149,-153,-57,156,-144,-145,156,-215,156,156,156,156,-57,-150,-155,-156,156,-146,-143,-58,]),'LAND':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,142,143,172,173,174,175,186,187,188,233,234,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,333,335,336,337,338,339,340,342,343,348,351,353,354,356,357,384,385,386,387,388,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,157,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,157,-58,157,-58,-143,237,239,-114,157,-133,-132,-134,-168,-169,-170,237,239,-127,-128,-129,-130,-131,-135,-136,-137,-138,157,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,157,157,-126,-58,157,157,157,-154,157,-55,-58,-58,157,157,-58,-115,-138,-118,237,239,-116,-117,239,382,157,-147,-148,-149,-153,-57,382,-122,-123,-124,-125,-144,-145,157,-215,157,-138,382,157,-57,-150,-155,-156,157,-146,-143,-58,]),'LOR':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,142,143,172,173,174,175,186,187,188,233,234,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,333,335,336,337,338,339,340,342,343,348,351,353,354,356,357,384,385,386,387,388,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,158,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,158,-58,158,-58,-143,238,240,-114,158,-133,-132,-134,-168,-169,-170,238,240,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,158,158,-126,-58,158,158,158,-154,158,-55,-58,-58,158,158,-58,-115,-138,-118,-139,-121,-116,-117,-119,-120,158,-147,-148,-149,-153,-57,383,-122,-123,-124,-125,-144,-145,158,-215,158,-138,-139,158,-57,-150,-155,-156,158,-146,-143,-58,]),'LSHIFT':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,159,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,159,-58,159,-58,-143,159,159,-133,-132,-134,159,159,159,159,-127,-128,-129,-130,-131,159,159,159,159,159,-140,-141,159,159,159,159,159,159,159,159,159,159,159,-126,-58,159,159,159,-154,159,-55,-58,-58,159,159,-58,159,159,159,159,159,-147,-148,-149,-153,-57,159,-144,-145,159,-215,159,159,159,159,-57,-150,-155,-156,159,-146,-143,-58,]),'RSHIFT':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,160,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,160,-58,160,-58,-143,160,160,-133,-132,-134,160,160,160,160,-127,-128,-129,-130,-131,160,160,160,160,160,-140,-141,160,160,160,160,160,160,160,160,160,160,160,-126,-58,160,160,160,-154,160,-55,-58,-58,160,160,-58,160,160,160,160,160,-147,-148,-149,-153,-57,160,-144,-145,160,-215,160,160,160,160,-57,-150,-155,-156,160,-146,-143,-58,]),'EQ':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,161,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,161,-58,161,-58,-143,161,161,-133,-132,-134,161,161,161,161,-127,-128,-129,-130,-131,161,161,161,161,161,-140,-141,-157,-158,-159,-160,-161,-162,161,161,161,161,161,-126,-58,161,161,161,-154,161,-55,-58,-58,161,161,-58,161,161,161,161,161,-147,-148,-149,-153,-57,161,-144,-145,161,-215,161,161,161,161,-57,-150,-155,-156,161,-146,-143,-58,]),'NE':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,162,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,162,-58,162,-58,-143,162,162,-133,-132,-134,162,162,162,162,-127,-128,-129,-130,-131,162,162,162,162,162,-140,-141,-157,-158,-159,-160,-161,-162,162,162,162,162,162,-126,-58,162,162,162,-154,162,-55,-58,-58,162,162,-58,162,162,162,162,162,-147,-148,-149,-153,-57,162,-144,-145,162,-215,162,162,162,162,-57,-150,-155,-156,162,-146,-143,-58,]),'LT':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,220,225,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,436,],[-60,-59,-183,163,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,163,-58,163,-58,-143,163,163,-133,-132,-134,163,163,163,317,327,163,-127,-128,-129,-130,-131,163,163,163,163,163,-140,-141,163,163,-159,-160,-161,-162,163,163,163,163,163,-126,-58,163,163,163,-154,163,-55,-58,-58,163,163,-58,163,163,163,163,163,-147,-148,-149,-153,-57,163,-144,-145,163,-215,163,163,163,163,-57,-150,-155,-156,163,-146,-143,-58,317,]),'LE':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,164,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,164,-58,164,-58,-143,164,164,-133,-132,-134,164,164,164,164,-127,-128,-129,-130,-131,164,164,164,164,164,-140,-141,164,164,-159,-160,-161,-162,164,164,164,164,164,-126,-58,164,164,164,-154,164,-55,-58,-58,164,164,-58,164,164,164,164,164,-147,-148,-149,-153,-57,164,-144,-145,164,-215,164,164,164,164,-57,-150,-155,-156,164,-146,-143,-58,]),'GT':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,315,318,323,325,335,337,340,343,348,351,353,354,356,357,370,377,384,390,391,392,393,403,405,406,412,413,414,415,416,417,418,419,424,425,428,432,433,],[-60,-59,-183,165,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,165,-58,165,-58,-143,165,165,-133,-132,-134,165,165,165,165,-127,-128,-129,-130,-131,165,165,165,165,165,-140,-141,165,165,-159,-160,-161,-162,165,165,165,165,165,-126,-58,165,165,165,-154,165,-55,-58,-58,165,-193,-195,165,-58,165,165,165,165,165,-147,-148,-149,-153,-57,402,409,165,-144,-145,165,-215,-196,-198,165,165,165,165,-57,-150,-155,-156,165,-197,-194,-146,-143,-58,]),'GE':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,166,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,166,-58,166,-58,-143,166,166,-133,-132,-134,166,166,166,166,-127,-128,-129,-130,-131,166,166,166,166,166,-140,-141,166,166,-159,-160,-161,-162,166,166,166,166,166,-126,-58,166,166,166,-154,166,-55,-58,-58,166,166,-58,166,166,166,166,166,-147,-148,-149,-153,-57,166,-144,-145,166,-215,166,166,166,166,-57,-150,-155,-156,166,-146,-143,-58,]),'UNTIL':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,167,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,167,-58,167,-58,-143,167,167,-133,-132,-134,-168,167,167,167,-127,-128,-129,-130,-131,-135,-136,-137,167,167,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,167,167,-126,-58,167,167,167,-154,167,-55,-58,-58,167,167,-58,167,167,167,167,167,-147,-148,-149,-153,-57,167,-144,-145,167,-215,167,167,167,167,-57,-150,-155,-156,167,-146,-143,-58,]),'WEAK_UNTIL':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,168,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,168,-58,168,-58,-143,168,168,-133,-132,-134,-168,168,168,168,-127,-128,-129,-130,-131,-135,-136,-137,168,168,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,168,168,-126,-58,168,168,168,-154,168,-55,-58,-58,168,168,-58,168,168,168,168,168,-147,-148,-149,-153,-57,168,-144,-145,168,-215,168,168,168,168,-57,-150,-155,-156,168,-146,-143,-58,]),'RELEASE':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,169,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,169,-58,169,-58,-143,169,169,-133,-132,-134,-168,169,169,169,-127,-128,-129,-130,-131,-135,-136,-137,169,169,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,169,169,-126,-58,169,169,169,-154,169,-55,-58,-58,169,169,-58,169,169,169,169,169,-147,-148,-149,-153,-57,169,-144,-145,169,-215,169,169,169,169,-57,-150,-155,-156,169,-146,-143,-58,]),'IMPLIES':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,170,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,170,-58,170,-58,-143,170,170,-133,-132,-134,-168,-169,-170,170,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,170,170,170,-154,170,-55,-58,-58,170,170,-58,-138,-139,170,170,170,-147,-148,-149,-153,-57,170,-144,-145,170,-215,170,-138,-139,170,-57,-150,-155,-156,170,-146,-143,-58,]),'EQUIV':([45,69,70,72,77,78,83,84,86,87,91,92,93,94,95,102,103,114,125,130,141,172,173,174,175,186,187,188,233,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,274,275,277,278,279,280,301,304,312,323,325,335,337,340,343,348,351,353,354,356,357,384,390,391,392,393,406,412,413,414,415,416,417,418,419,428,432,433,],[-60,-59,-183,171,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,171,-58,171,-58,-143,171,171,-133,-132,-134,-168,-169,-170,171,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,171,171,171,-154,171,-55,-58,-58,171,171,-58,-138,-139,171,171,171,-147,-148,-149,-153,-57,171,-144,-145,171,-215,171,-138,-139,171,-57,-150,-155,-156,171,-146,-143,-58,]),'RBRACKET':([45,69,70,77,78,83,84,86,87,91,92,93,94,95,102,103,109,110,173,174,175,186,187,188,204,206,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,279,280,287,288,289,290,291,292,315,318,349,350,351,353,354,356,357,390,391,392,393,403,405,415,416,417,418,424,425,428,],[-60,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,194,195,198,-171,-133,-132,-134,-168,-169,-170,-172,293,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,357,-55,-173,-174,-175,-176,-177,-178,-193,-195,390,391,-147,-148,-149,-153,-57,-144,-145,415,-215,-196,-198,-57,-150,-155,-156,-197,-194,-146,]),'UNLESS':([45,69,70,77,78,83,84,86,87,91,92,93,94,95,121,122,124,125,128,129,130,131,135,137,141,142,143,173,174,175,186,187,188,213,214,216,220,223,224,227,232,235,245,246,247,248,249,250,251,252,253,254,255,256,257,258,259,260,261,262,263,264,265,266,267,268,273,278,280,297,298,301,302,303,304,308,312,315,316,318,321,322,323,324,325,326,328,329,332,333,335,336,337,338,339,340,342,343,351,353,354,356,357,364,365,366,385,386,387,388,390,391,393,399,400,401,402,403,405,409,410,412,413,415,416,417,418,424,425,426,428,432,433,434,],[-60,-59,-183,-142,-143,-151,-152,-58,-56,-179,-180,-54,-181,-182,-92,-94,215,-58,-79,-80,-143,-103,-90,-91,-112,-113,-114,-133,-132,-134,-168,-169,-170,-92,-94,-106,-101,-82,-83,-104,-84,-99,-127,-128,-129,-130,-131,-135,-136,-137,-138,-139,-140,-141,-157,-158,-159,-160,-161,-162,-163,-164,-165,-166,-167,-126,-58,-154,-55,-92,-94,-58,-92,-94,-58,-105,-191,-193,-85,-195,-102,-189,-191,-81,-58,-87,-89,-107,-108,-115,-138,-118,-139,-121,-116,-117,-119,-120,-147,-148,-149,-153,-57,-96,-106,-97,-122,-123,-124,-125,-144,-145,-215,-192,-93,-95,-86,-196,-198,-88,-100,-138,-139,-57,-150,-155,-156,-197,-194,-190,-146,-143,-58,-98,]),'RCV':([78,86,87,93,103,125,130,273,280,301,304,325,357,415,432,433,],[176,-58,-56,-54,-58,-58,220,-58,-55,-58,-58,-58,-57,-57,436,-58,]),'R_RCV':([78,86,87,93,103,125,130,273,280,301,304,325,357,415,432,433,],[177,-58,-56,-54,-58,-58,225,-58,-55,-58,-58,-58,-57,-57,225,-58,]),'AT':([86,103,125,301,304,325,357,433,],[184,184,184,184,184,184,394,184,]),'PERIOD':([86,87,93,103,125,273,280,301,304,325,357,415,433,],[-58,-56,189,-58,-58,-58,-55,-58,-58,-58,-57,-57,-58,]),'INCR':([87,93,125,130,273,280,301,304,357,415,432,433,],[-56,-54,-58,223,-58,-55,-58,-58,-57,-57,223,-58,]),'DECR':([87,93,125,130,273,280,301,304,357,415,432,433,],[-56,-54,-58,224,-58,-55,-58,-58,-57,-57,224,-58,]),'TX2':([87,93,125,130,273,280,301,304,357,415,432,433,],[-56,-54,-58,226,-58,-55,-58,-58,-57,-57,226,-58,]),'XR':([216,],[306,]),'XS':([216,],[307,]),'EVAL':([220,225,270,271,317,319,327,371,372,436,],[320,320,320,320,320,320,320,320,320,320,]),'STRING':([236,],[334,]),'OF':([293,],[363,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
@@ -22,223 +22,223 @@
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> program","S'",1,None,None,None),
-  ('program -> units','program',1,'p_program','yacc.py',115),
-  ('units -> units unit','units',2,'p_units_iter','yacc.py',119),
-  ('units -> unit','units',1,'p_units_end','yacc.py',123),
-  ('unit -> proc','unit',1,'p_unit_proc','yacc.py',128),
-  ('unit -> init','unit',1,'p_unit_proc','yacc.py',129),
-  ('unit -> claim','unit',1,'p_unit_proc','yacc.py',130),
-  ('unit -> ltl','unit',1,'p_unit_proc','yacc.py',131),
-  ('unit -> one_decl','unit',1,'p_unit_decl','yacc.py',136),
-  ('unit -> utype','unit',1,'p_unit_decl','yacc.py',137),
-  ('unit -> semi','unit',1,'p_unit_semi','yacc.py',142),
-  ('proc -> prefix_proctype NAME LPAREN decl RPAREN opt_priority opt_enabler body','proc',8,'p_proc','yacc.py',145),
-  ('prefix_proctype -> ACTIVE opt_index proctype','prefix_proctype',3,'p_inst','yacc.py',163),
-  ('prefix_proctype -> proctype','prefix_proctype',1,'p_inactive_proctype','yacc.py',173),
-  ('opt_index -> LBRACKET expr RBRACKET','opt_index',3,'p_opt_index','yacc.py',177),
-  ('opt_index -> LBRACKET NAME RBRACKET','opt_index',3,'p_opt_index','yacc.py',178),
-  ('opt_index -> empty','opt_index',1,'p_opt_index_empty','yacc.py',183),
-  ('init -> INIT opt_priority body','init',3,'p_init','yacc.py',186),
-  ('claim -> CLAIM optname body','claim',3,'p_claim','yacc.py',190),
-  ('utype -> TYPEDEF NAME LBRACE decl_lst RBRACE','utype',5,'p_utype','yacc.py',196),
-  ('ltl -> LTL LBRACE expr RBRACE','ltl',4,'p_ltl','yacc.py',201),
-  ('decl -> decl_lst','decl',1,'p_decl','yacc.py',208),
-  ('decl -> empty','decl',1,'p_decl_empty','yacc.py',212),
-  ('decl_lst -> one_decl SEMI decl_lst','decl_lst',3,'p_decl_lst_iter','yacc.py',215),
-  ('decl_lst -> one_decl','decl_lst',1,'p_decl_lst_end','yacc.py',219),
-  ('one_decl -> vis typename var_list','one_decl',3,'p_one_decl_visible','yacc.py',223),
-  ('one_decl -> vis NAME var_list','one_decl',3,'p_one_decl_visible','yacc.py',224),
-  ('one_decl -> typename var_list','one_decl',2,'p_one_decl','yacc.py',233),
-  ('one_decl -> NAME var_list','one_decl',2,'p_one_decl','yacc.py',234),
-  ('one_decl -> vis MTYPE asgn LBRACE name_list RBRACE','one_decl',6,'p_one_decl_mtype_vis','yacc.py',249),
-  ('one_decl -> MTYPE asgn LBRACE name_list RBRACE','one_decl',5,'p_one_decl_mtype','yacc.py',253),
-  ('name_list -> name_list COMMA NAME','name_list',3,'p_name_list_iter','yacc.py',257),
-  ('name_list -> NAME','name_list',1,'p_name_list_end','yacc.py',262),
-  ('var_list -> ivar COMMA var_list','var_list',3,'p_var_list_iter','yacc.py',266),
-  ('var_list -> ivar','var_list',1,'p_var_list_end','yacc.py',270),
-  ('ivar -> vardcl','ivar',1,'p_ivar','yacc.py',277),
-  ('ivar -> vardcl asgn expr','ivar',3,'p_ivar_asgn','yacc.py',281),
-  ('vardcl -> NAME','vardcl',1,'p_vardcl','yacc.py',287),
-  ('vardcl -> NAME COLON const','vardcl',3,'p_vardcl_unsigned','yacc.py',292),
-  ('vardcl -> NAME LBRACKET const_expr RBRACKET','vardcl',4,'p_vardcl_array','yacc.py',296),
-  ('vardcl -> vardcl EQUALS ch_init','vardcl',3,'p_vardcl_chan','yacc.py',300),
-  ('typename -> BIT','typename',1,'p_typename','yacc.py',305),
-  ('typename -> BOOL','typename',1,'p_typename','yacc.py',306),
-  ('typename -> BYTE','typename',1,'p_typename','yacc.py',307),
-  ('typename -> CHAN','typename',1,'p_typename','yacc.py',308),
-  ('typename -> INT','typename',1,'p_typename','yacc.py',309),
-  ('typename -> PID','typename',1,'p_typename','yacc.py',310),
-  ('typename -> SHORT','typename',1,'p_typename','yacc.py',311),
-  ('typename -> UNSIGNED','typename',1,'p_typename','yacc.py',312),
-  ('typename -> MTYPE','typename',1,'p_typename','yacc.py',313),
-  ('ch_init -> LBRACKET const_expr RBRACKET OF LBRACE typ_list RBRACE','ch_init',7,'p_ch_init','yacc.py',318),
-  ('typ_list -> typ_list COMMA basetype','typ_list',3,'p_typ_list_iter','yacc.py',323),
-  ('typ_list -> basetype','typ_list',1,'p_typ_list_end','yacc.py',328),
-  ('basetype -> typename','basetype',1,'p_basetype','yacc.py',333),
-  ('varref -> cmpnd','varref',1,'p_varref','yacc.py',340),
-  ('cmpnd -> cmpnd PERIOD cmpnd','cmpnd',3,'p_cmpnd_iter','yacc.py',344),
-  ('cmpnd -> pfld','cmpnd',1,'p_cmpnd_end','yacc.py',348),
-  ('pfld -> NAME LBRACKET expr RBRACKET','pfld',4,'p_pfld_indexed','yacc.py',353),
-  ('pfld -> NAME','pfld',1,'p_pfld','yacc.py',357),
-  ('opt_priority -> PRIORITY number','opt_priority',2,'p_opt_priority','yacc.py',364),
-  ('opt_priority -> empty','opt_priority',1,'p_opt_priority_empty','yacc.py',368),
-  ('opt_enabler -> PROVIDED LPAREN expr RPAREN','opt_enabler',4,'p_opt_enabler','yacc.py',371),
-  ('opt_enabler -> empty','opt_enabler',1,'p_opt_enabler_empty','yacc.py',375),
-  ('body -> LBRACE sequence os RBRACE','body',4,'p_body','yacc.py',378),
-  ('sequence -> sequence msemi step','sequence',3,'p_sequence','yacc.py',385),
-  ('sequence -> seq_block step','sequence',2,'p_sequence_ending_with_atomic','yacc.py',390),
-  ('sequence -> step','sequence',1,'p_sequence_single','yacc.py',395),
-  ('seq_block -> sequence msemi atomic','seq_block',3,'p_seq_block','yacc.py',399),
-  ('seq_block -> sequence msemi dstep','seq_block',3,'p_seq_block','yacc.py',400),
-  ('seq_block -> seq_block atomic','seq_block',2,'p_seq_block_iter','yacc.py',406),
-  ('seq_block -> seq_block dstep','seq_block',2,'p_seq_block_iter','yacc.py',407),
-  ('seq_block -> atomic','seq_block',1,'p_seq_block_single','yacc.py',413),
-  ('seq_block -> dstep','seq_block',1,'p_seq_block_single','yacc.py',414),
-  ('step -> one_decl','step',1,'p_step_1','yacc.py',420),
-  ('step -> stmnt','step',1,'p_step_1','yacc.py',421),
-  ('step -> NAME COLON one_decl','step',3,'p_step_labeled','yacc.py',426),
-  ('step -> NAME COLON XR','step',3,'p_step_3','yacc.py',431),
-  ('step -> NAME COLON XS','step',3,'p_step_3','yacc.py',432),
-  ('step -> stmnt UNLESS stmnt','step',3,'p_step_4','yacc.py',438),
-  ('stmnt -> special','stmnt',1,'p_stmnt','yacc.py',446),
-  ('stmnt -> statement','stmnt',1,'p_stmnt','yacc.py',447),
-  ('statement -> varref asgn full_expr','statement',3,'p_statement_asgn','yacc.py',453),
-  ('statement -> varref INCR','statement',2,'p_statement_incr','yacc.py',457),
-  ('statement -> varref DECR','statement',2,'p_statement_decr','yacc.py',463),
-  ('statement -> ASSERT full_expr','statement',2,'p_statement_assert','yacc.py',469),
-  ('statement -> varref RCV rargs','statement',3,'p_statement_fifo_receive','yacc.py',473),
-  ('statement -> varref RCV LT rargs GT','statement',5,'p_statement_copy_fifo_receive','yacc.py',477),
-  ('statement -> varref R_RCV rargs','statement',3,'p_statement_random_receive','yacc.py',481),
-  ('statement -> varref R_RCV LT rargs GT','statement',5,'p_statement_copy_random_receive','yacc.py',485),
-  ('statement -> varref TX2 margs','statement',3,'p_statement_tx2','yacc.py',489),
-  ('statement -> full_expr','statement',1,'p_statement_full_expr','yacc.py',493),
-  ('statement -> ELSE','statement',1,'p_statement_else','yacc.py',497),
-  ('statement -> atomic','statement',1,'p_statement_atomic','yacc.py',501),
-  ('atomic -> ATOMIC LBRACE sequence os RBRACE','atomic',5,'p_atomic','yacc.py',505),
-  ('statement -> dstep','statement',1,'p_statement_dstep','yacc.py',511),
-  ('dstep -> D_STEP LBRACE sequence os RBRACE','dstep',5,'p_dstep','yacc.py',515),
-  ('statement -> LBRACE sequence os RBRACE','statement',4,'p_statement_braces','yacc.py',521),
-  ('statement -> NAME LPAREN args RPAREN','statement',4,'p_statement_call','yacc.py',526),
-  ('statement -> varref asgn NAME LPAREN args RPAREN statement','statement',7,'p_statement_assgn_call','yacc.py',532),
-  ('statement -> RETURN full_expr','statement',2,'p_statement_return','yacc.py',537),
-  ('statement -> PRINT LPAREN STRING prargs RPAREN','statement',5,'p_printf','yacc.py',541),
-  ('special -> varref RCV','special',2,'p_special','yacc.py',554),
-  ('special -> varref LNOT margs','special',3,'p_varref_lnot','yacc.py',558),
-  ('special -> BREAK','special',1,'p_break','yacc.py',562),
-  ('special -> GOTO NAME','special',2,'p_goto','yacc.py',566),
-  ('special -> NAME COLON stmnt','special',3,'p_labeled_stmt','yacc.py',570),
-  ('special -> NAME COLON','special',2,'p_labeled','yacc.py',574),
-  ('special -> IF options FI','special',3,'p_special_if','yacc.py',580),
-  ('special -> DO options OD','special',3,'p_special_do','yacc.py',584),
-  ('options -> option','options',1,'p_options_end','yacc.py',588),
-  ('options -> options option','options',2,'p_options_iter','yacc.py',592),
-  ('option -> COLONS sequence os','option',3,'p_option','yacc.py',597),
-  ('full_expr -> expr','full_expr',1,'p_full_expr','yacc.py',606),
-  ('full_expr -> pexpr','full_expr',1,'p_full_expr','yacc.py',607),
-  ('pexpr -> probe','pexpr',1,'p_pexpr','yacc.py',613),
-  ('pexpr -> LPAREN pexpr RPAREN','pexpr',3,'p_pexpr','yacc.py',614),
-  ('pexpr -> pexpr LAND pexpr','pexpr',3,'p_pexpr','yacc.py',615),
-  ('pexpr -> pexpr LAND expr','pexpr',3,'p_pexpr','yacc.py',616),
-  ('pexpr -> expr LAND pexpr','pexpr',3,'p_pexpr','yacc.py',617),
-  ('pexpr -> pexpr LOR pexpr','pexpr',3,'p_pexpr','yacc.py',618),
-  ('pexpr -> pexpr LOR expr','pexpr',3,'p_pexpr','yacc.py',619),
-  ('pexpr -> expr LOR pexpr','pexpr',3,'p_pexpr','yacc.py',620),
-  ('probe -> FULL LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',625),
-  ('probe -> NFULL LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',626),
-  ('probe -> EMPTY LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',627),
-  ('probe -> NEMPTY LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',628),
-  ('expr -> LPAREN expr RPAREN','expr',3,'p_expr_paren','yacc.py',633),
-  ('expr -> expr PLUS expr','expr',3,'p_expr_arithmetic','yacc.py',637),
-  ('expr -> expr MINUS expr','expr',3,'p_expr_arithmetic','yacc.py',638),
-  ('expr -> expr TIMES expr','expr',3,'p_expr_arithmetic','yacc.py',639),
-  ('expr -> expr DIVIDE expr','expr',3,'p_expr_arithmetic','yacc.py',640),
-  ('expr -> expr MOD expr','expr',3,'p_expr_arithmetic','yacc.py',641),
-  ('expr -> NOT expr','expr',2,'p_expr_not','yacc.py',646),
-  ('expr -> MINUS expr','expr',2,'p_expr_not','yacc.py',647),
-  ('expr -> LNOT expr','expr',2,'p_expr_not','yacc.py',648),
-  ('expr -> expr AND expr','expr',3,'p_expr_logical','yacc.py',653),
-  ('expr -> expr OR expr','expr',3,'p_expr_logical','yacc.py',654),
-  ('expr -> expr XOR expr','expr',3,'p_expr_logical','yacc.py',655),
-  ('expr -> expr LAND expr','expr',3,'p_expr_logical','yacc.py',656),
-  ('expr -> expr LOR expr','expr',3,'p_expr_logical','yacc.py',657),
-  ('expr -> expr LSHIFT expr','expr',3,'p_expr_shift','yacc.py',664),
-  ('expr -> expr RSHIFT expr','expr',3,'p_expr_shift','yacc.py',665),
-  ('expr -> const','expr',1,'p_expr_const_varref','yacc.py',670),
-  ('expr -> varref','expr',1,'p_expr_const_varref','yacc.py',671),
-  ('expr -> varref RCV LBRACKET rargs RBRACKET','expr',5,'p_expr_varref','yacc.py',676),
-  ('expr -> varref R_RCV LBRACKET rargs RBRACKET','expr',5,'p_expr_varref','yacc.py',677),
-  ('expr -> LPAREN expr ARROW expr COLON expr RPAREN','expr',7,'p_expr_other','yacc.py',683),
-  ('expr -> LEN LPAREN varref RPAREN','expr',4,'p_expr_other','yacc.py',684),
-  ('expr -> ENABLED LPAREN expr RPAREN','expr',4,'p_expr_other','yacc.py',685),
-  ('expr -> GET_P LPAREN expr RPAREN','expr',4,'p_expr_other','yacc.py',686),
-  ('expr -> RUN aname LPAREN args RPAREN opt_priority','expr',6,'p_expr_run','yacc.py',692),
-  ('expr -> TIMEOUT','expr',1,'p_expr_other_2','yacc.py',696),
-  ('expr -> NONPROGRESS','expr',1,'p_expr_other_2','yacc.py',697),
-  ('expr -> PC_VAL LPAREN expr RPAREN','expr',4,'p_expr_other_2','yacc.py',698),
-  ('expr -> NAME AT NAME','expr',3,'p_expr_remote_ref_proctype_pc','yacc.py',703),
-  ('expr -> NAME LBRACKET expr RBRACKET AT NAME','expr',6,'p_expr_remote_ref_pid_pc','yacc.py',708),
-  ('expr -> NAME LBRACKET expr RBRACKET COLON pfld','expr',6,'p_expr_remote_ref_var','yacc.py',712),
-  ('expr -> expr EQ expr','expr',3,'p_expr_comparator','yacc.py',717),
-  ('expr -> expr NE expr','expr',3,'p_expr_comparator','yacc.py',718),
-  ('expr -> expr LT expr','expr',3,'p_expr_comparator','yacc.py',719),
-  ('expr -> expr LE expr','expr',3,'p_expr_comparator','yacc.py',720),
-  ('expr -> expr GT expr','expr',3,'p_expr_comparator','yacc.py',721),
-  ('expr -> expr GE expr','expr',3,'p_expr_comparator','yacc.py',722),
-  ('expr -> expr UNTIL expr','expr',3,'p_binary_ltl_expr','yacc.py',727),
-  ('expr -> expr WEAK_UNTIL expr','expr',3,'p_binary_ltl_expr','yacc.py',728),
-  ('expr -> expr RELEASE expr','expr',3,'p_binary_ltl_expr','yacc.py',729),
-  ('expr -> expr IMPLIES expr','expr',3,'p_binary_ltl_expr','yacc.py',730),
-  ('expr -> expr EQUIV expr','expr',3,'p_binary_ltl_expr','yacc.py',731),
-  ('expr -> NEXT expr','expr',2,'p_unary_ltl_expr','yacc.py',736),
-  ('expr -> ALWAYS expr','expr',2,'p_unary_ltl_expr','yacc.py',737),
-  ('expr -> EVENTUALLY expr','expr',2,'p_unary_ltl_expr','yacc.py',738),
-  ('const_expr -> const','const_expr',1,'p_const_expr_const','yacc.py',746),
-  ('const_expr -> MINUS const_expr','const_expr',2,'p_const_expr_unary','yacc.py',750),
-  ('const_expr -> const_expr PLUS const_expr','const_expr',3,'p_const_expr_binary','yacc.py',754),
-  ('const_expr -> const_expr MINUS const_expr','const_expr',3,'p_const_expr_binary','yacc.py',755),
-  ('const_expr -> const_expr TIMES const_expr','const_expr',3,'p_const_expr_binary','yacc.py',756),
-  ('const_expr -> const_expr DIVIDE const_expr','const_expr',3,'p_const_expr_binary','yacc.py',757),
-  ('const_expr -> const_expr MOD const_expr','const_expr',3,'p_const_expr_binary','yacc.py',758),
-  ('const_expr -> LPAREN const_expr RPAREN','const_expr',3,'p_const_expr_paren','yacc.py',763),
-  ('const -> boolean','const',1,'p_const','yacc.py',767),
-  ('const -> number','const',1,'p_const','yacc.py',768),
-  ('boolean -> TRUE','boolean',1,'p_bool','yacc.py',774),
-  ('boolean -> FALSE','boolean',1,'p_bool','yacc.py',775),
-  ('number -> INTEGER','number',1,'p_number','yacc.py',780),
-  ('two_args -> expr COMMA expr','two_args',3,'p_two_args','yacc.py',787),
-  ('args -> arg','args',1,'p_args','yacc.py',790),
-  ('prargs -> COMMA arg','prargs',2,'p_prargs','yacc.py',794),
-  ('prargs -> empty','prargs',1,'p_prargs_empty','yacc.py',798),
-  ('args -> empty','args',1,'p_args_empty','yacc.py',801),
-  ('margs -> arg','margs',1,'p_margs','yacc.py',804),
-  ('margs -> expr LPAREN arg RPAREN','margs',4,'p_margs','yacc.py',805),
-  ('arg -> expr','arg',1,'p_arg','yacc.py',809),
-  ('arg -> expr COMMA arg','arg',3,'p_arg','yacc.py',810),
-  ('rarg -> varref','rarg',1,'p_rarg','yacc.py',816),
-  ('rarg -> EVAL LPAREN expr RPAREN','rarg',4,'p_rarg','yacc.py',817),
-  ('rargs -> rarg','rargs',1,'p_rargs','yacc.py',822),
-  ('rargs -> rarg COMMA rargs','rargs',3,'p_rargs','yacc.py',823),
-  ('rargs -> rarg LPAREN rargs RPAREN','rargs',4,'p_rargs','yacc.py',824),
-  ('rargs -> LPAREN rargs RPAREN','rargs',3,'p_rargs','yacc.py',825),
-  ('proctype -> PROCTYPE','proctype',1,'p_proctype','yacc.py',829),
-  ('proctype -> D_PROCTYPE','proctype',1,'p_proctype','yacc.py',830),
-  ('aname -> NAME','aname',1,'p_aname','yacc.py',839),
-  ('optname -> NAME','optname',1,'p_optname','yacc.py',844),
-  ('optname -> empty','optname',1,'p_optname_empty','yacc.py',848),
-  ('os -> empty','os',1,'p_os','yacc.py',852),
-  ('os -> semi','os',1,'p_os','yacc.py',853),
-  ('msemi -> semi','msemi',1,'p_msemi','yacc.py',859),
-  ('msemi -> msemi semi','msemi',2,'p_msemi','yacc.py',860),
-  ('semi -> SEMI','semi',1,'p_semi','yacc.py',865),
-  ('semi -> ARROW','semi',1,'p_semi','yacc.py',866),
-  ('asgn -> EQUALS','asgn',1,'p_asgn','yacc.py',871),
-  ('asgn -> empty','asgn',1,'p_asgn','yacc.py',872),
-  ('vis -> HIDDEN','vis',1,'p_visible','yacc.py',877),
-  ('vis -> SHOW','vis',1,'p_visible','yacc.py',878),
-  ('vis -> ISLOCAL','vis',1,'p_visible','yacc.py',879),
-  ('empty -> <empty>','empty',0,'p_empty','yacc.py',884),
+  ('program -> units','program',1,'p_program','yacc.py',118),
+  ('units -> units unit','units',2,'p_units_iter','yacc.py',122),
+  ('units -> unit','units',1,'p_units_end','yacc.py',126),
+  ('unit -> proc','unit',1,'p_unit_proc','yacc.py',131),
+  ('unit -> init','unit',1,'p_unit_proc','yacc.py',132),
+  ('unit -> claim','unit',1,'p_unit_proc','yacc.py',133),
+  ('unit -> ltl','unit',1,'p_unit_proc','yacc.py',134),
+  ('unit -> one_decl','unit',1,'p_unit_decl','yacc.py',139),
+  ('unit -> utype','unit',1,'p_unit_decl','yacc.py',140),
+  ('unit -> semi','unit',1,'p_unit_semi','yacc.py',145),
+  ('proc -> prefix_proctype NAME LPAREN decl RPAREN opt_priority opt_enabler body','proc',8,'p_proc','yacc.py',148),
+  ('prefix_proctype -> ACTIVE opt_index proctype','prefix_proctype',3,'p_inst','yacc.py',166),
+  ('prefix_proctype -> proctype','prefix_proctype',1,'p_inactive_proctype','yacc.py',176),
+  ('opt_index -> LBRACKET expr RBRACKET','opt_index',3,'p_opt_index','yacc.py',180),
+  ('opt_index -> LBRACKET NAME RBRACKET','opt_index',3,'p_opt_index','yacc.py',181),
+  ('opt_index -> empty','opt_index',1,'p_opt_index_empty','yacc.py',186),
+  ('init -> INIT opt_priority body','init',3,'p_init','yacc.py',189),
+  ('claim -> CLAIM optname body','claim',3,'p_claim','yacc.py',193),
+  ('utype -> TYPEDEF NAME LBRACE decl_lst RBRACE','utype',5,'p_utype','yacc.py',199),
+  ('ltl -> LTL LBRACE expr RBRACE','ltl',4,'p_ltl','yacc.py',204),
+  ('decl -> decl_lst','decl',1,'p_decl','yacc.py',211),
+  ('decl -> empty','decl',1,'p_decl_empty','yacc.py',215),
+  ('decl_lst -> one_decl SEMI decl_lst','decl_lst',3,'p_decl_lst_iter','yacc.py',218),
+  ('decl_lst -> one_decl','decl_lst',1,'p_decl_lst_end','yacc.py',222),
+  ('one_decl -> vis typename var_list','one_decl',3,'p_one_decl_visible','yacc.py',226),
+  ('one_decl -> vis NAME var_list','one_decl',3,'p_one_decl_visible','yacc.py',227),
+  ('one_decl -> typename var_list','one_decl',2,'p_one_decl','yacc.py',236),
+  ('one_decl -> NAME var_list','one_decl',2,'p_one_decl','yacc.py',237),
+  ('one_decl -> vis MTYPE asgn LBRACE name_list RBRACE','one_decl',6,'p_one_decl_mtype_vis','yacc.py',252),
+  ('one_decl -> MTYPE asgn LBRACE name_list RBRACE','one_decl',5,'p_one_decl_mtype','yacc.py',256),
+  ('name_list -> name_list COMMA NAME','name_list',3,'p_name_list_iter','yacc.py',260),
+  ('name_list -> NAME','name_list',1,'p_name_list_end','yacc.py',265),
+  ('var_list -> ivar COMMA var_list','var_list',3,'p_var_list_iter','yacc.py',269),
+  ('var_list -> ivar','var_list',1,'p_var_list_end','yacc.py',273),
+  ('ivar -> vardcl','ivar',1,'p_ivar','yacc.py',280),
+  ('ivar -> vardcl asgn expr','ivar',3,'p_ivar_asgn','yacc.py',284),
+  ('vardcl -> NAME','vardcl',1,'p_vardcl','yacc.py',290),
+  ('vardcl -> NAME COLON const','vardcl',3,'p_vardcl_unsigned','yacc.py',295),
+  ('vardcl -> NAME LBRACKET const_expr RBRACKET','vardcl',4,'p_vardcl_array','yacc.py',299),
+  ('vardcl -> vardcl EQUALS ch_init','vardcl',3,'p_vardcl_chan','yacc.py',303),
+  ('typename -> BIT','typename',1,'p_typename','yacc.py',308),
+  ('typename -> BOOL','typename',1,'p_typename','yacc.py',309),
+  ('typename -> BYTE','typename',1,'p_typename','yacc.py',310),
+  ('typename -> CHAN','typename',1,'p_typename','yacc.py',311),
+  ('typename -> INT','typename',1,'p_typename','yacc.py',312),
+  ('typename -> PID','typename',1,'p_typename','yacc.py',313),
+  ('typename -> SHORT','typename',1,'p_typename','yacc.py',314),
+  ('typename -> UNSIGNED','typename',1,'p_typename','yacc.py',315),
+  ('typename -> MTYPE','typename',1,'p_typename','yacc.py',316),
+  ('ch_init -> LBRACKET const_expr RBRACKET OF LBRACE typ_list RBRACE','ch_init',7,'p_ch_init','yacc.py',321),
+  ('typ_list -> typ_list COMMA basetype','typ_list',3,'p_typ_list_iter','yacc.py',326),
+  ('typ_list -> basetype','typ_list',1,'p_typ_list_end','yacc.py',331),
+  ('basetype -> typename','basetype',1,'p_basetype','yacc.py',336),
+  ('varref -> cmpnd','varref',1,'p_varref','yacc.py',343),
+  ('cmpnd -> cmpnd PERIOD cmpnd','cmpnd',3,'p_cmpnd_iter','yacc.py',347),
+  ('cmpnd -> pfld','cmpnd',1,'p_cmpnd_end','yacc.py',351),
+  ('pfld -> NAME LBRACKET expr RBRACKET','pfld',4,'p_pfld_indexed','yacc.py',356),
+  ('pfld -> NAME','pfld',1,'p_pfld','yacc.py',360),
+  ('opt_priority -> PRIORITY number','opt_priority',2,'p_opt_priority','yacc.py',367),
+  ('opt_priority -> empty','opt_priority',1,'p_opt_priority_empty','yacc.py',371),
+  ('opt_enabler -> PROVIDED LPAREN expr RPAREN','opt_enabler',4,'p_opt_enabler','yacc.py',374),
+  ('opt_enabler -> empty','opt_enabler',1,'p_opt_enabler_empty','yacc.py',378),
+  ('body -> LBRACE sequence os RBRACE','body',4,'p_body','yacc.py',381),
+  ('sequence -> sequence msemi step','sequence',3,'p_sequence','yacc.py',388),
+  ('sequence -> seq_block step','sequence',2,'p_sequence_ending_with_atomic','yacc.py',393),
+  ('sequence -> step','sequence',1,'p_sequence_single','yacc.py',398),
+  ('seq_block -> sequence msemi atomic','seq_block',3,'p_seq_block','yacc.py',402),
+  ('seq_block -> sequence msemi dstep','seq_block',3,'p_seq_block','yacc.py',403),
+  ('seq_block -> seq_block atomic','seq_block',2,'p_seq_block_iter','yacc.py',409),
+  ('seq_block -> seq_block dstep','seq_block',2,'p_seq_block_iter','yacc.py',410),
+  ('seq_block -> atomic','seq_block',1,'p_seq_block_single','yacc.py',416),
+  ('seq_block -> dstep','seq_block',1,'p_seq_block_single','yacc.py',417),
+  ('step -> one_decl','step',1,'p_step_1','yacc.py',423),
+  ('step -> stmnt','step',1,'p_step_1','yacc.py',424),
+  ('step -> NAME COLON one_decl','step',3,'p_step_labeled','yacc.py',429),
+  ('step -> NAME COLON XR','step',3,'p_step_3','yacc.py',434),
+  ('step -> NAME COLON XS','step',3,'p_step_3','yacc.py',435),
+  ('step -> stmnt UNLESS stmnt','step',3,'p_step_4','yacc.py',441),
+  ('stmnt -> special','stmnt',1,'p_stmnt','yacc.py',449),
+  ('stmnt -> statement','stmnt',1,'p_stmnt','yacc.py',450),
+  ('statement -> varref asgn full_expr','statement',3,'p_statement_asgn','yacc.py',456),
+  ('statement -> varref INCR','statement',2,'p_statement_incr','yacc.py',460),
+  ('statement -> varref DECR','statement',2,'p_statement_decr','yacc.py',466),
+  ('statement -> ASSERT full_expr','statement',2,'p_statement_assert','yacc.py',472),
+  ('statement -> varref RCV rargs','statement',3,'p_statement_fifo_receive','yacc.py',476),
+  ('statement -> varref RCV LT rargs GT','statement',5,'p_statement_copy_fifo_receive','yacc.py',480),
+  ('statement -> varref R_RCV rargs','statement',3,'p_statement_random_receive','yacc.py',484),
+  ('statement -> varref R_RCV LT rargs GT','statement',5,'p_statement_copy_random_receive','yacc.py',488),
+  ('statement -> varref TX2 margs','statement',3,'p_statement_tx2','yacc.py',492),
+  ('statement -> full_expr','statement',1,'p_statement_full_expr','yacc.py',496),
+  ('statement -> ELSE','statement',1,'p_statement_else','yacc.py',500),
+  ('statement -> atomic','statement',1,'p_statement_atomic','yacc.py',504),
+  ('atomic -> ATOMIC LBRACE sequence os RBRACE','atomic',5,'p_atomic','yacc.py',508),
+  ('statement -> dstep','statement',1,'p_statement_dstep','yacc.py',514),
+  ('dstep -> D_STEP LBRACE sequence os RBRACE','dstep',5,'p_dstep','yacc.py',518),
+  ('statement -> LBRACE sequence os RBRACE','statement',4,'p_statement_braces','yacc.py',524),
+  ('statement -> NAME LPAREN args RPAREN','statement',4,'p_statement_call','yacc.py',529),
+  ('statement -> varref asgn NAME LPAREN args RPAREN statement','statement',7,'p_statement_assgn_call','yacc.py',535),
+  ('statement -> RETURN full_expr','statement',2,'p_statement_return','yacc.py',540),
+  ('statement -> PRINT LPAREN STRING prargs RPAREN','statement',5,'p_printf','yacc.py',544),
+  ('special -> varref RCV','special',2,'p_special','yacc.py',557),
+  ('special -> varref LNOT margs','special',3,'p_varref_lnot','yacc.py',561),
+  ('special -> BREAK','special',1,'p_break','yacc.py',565),
+  ('special -> GOTO NAME','special',2,'p_goto','yacc.py',569),
+  ('special -> NAME COLON stmnt','special',3,'p_labeled_stmt','yacc.py',573),
+  ('special -> NAME COLON','special',2,'p_labeled','yacc.py',577),
+  ('special -> IF options FI','special',3,'p_special_if','yacc.py',583),
+  ('special -> DO options OD','special',3,'p_special_do','yacc.py',587),
+  ('options -> option','options',1,'p_options_end','yacc.py',591),
+  ('options -> options option','options',2,'p_options_iter','yacc.py',595),
+  ('option -> COLONS sequence os','option',3,'p_option','yacc.py',600),
+  ('full_expr -> expr','full_expr',1,'p_full_expr','yacc.py',609),
+  ('full_expr -> pexpr','full_expr',1,'p_full_expr','yacc.py',610),
+  ('pexpr -> probe','pexpr',1,'p_pexpr','yacc.py',616),
+  ('pexpr -> LPAREN pexpr RPAREN','pexpr',3,'p_pexpr','yacc.py',617),
+  ('pexpr -> pexpr LAND pexpr','pexpr',3,'p_pexpr','yacc.py',618),
+  ('pexpr -> pexpr LAND expr','pexpr',3,'p_pexpr','yacc.py',619),
+  ('pexpr -> expr LAND pexpr','pexpr',3,'p_pexpr','yacc.py',620),
+  ('pexpr -> pexpr LOR pexpr','pexpr',3,'p_pexpr','yacc.py',621),
+  ('pexpr -> pexpr LOR expr','pexpr',3,'p_pexpr','yacc.py',622),
+  ('pexpr -> expr LOR pexpr','pexpr',3,'p_pexpr','yacc.py',623),
+  ('probe -> FULL LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',628),
+  ('probe -> NFULL LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',629),
+  ('probe -> EMPTY LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',630),
+  ('probe -> NEMPTY LPAREN varref RPAREN','probe',4,'p_probe','yacc.py',631),
+  ('expr -> LPAREN expr RPAREN','expr',3,'p_expr_paren','yacc.py',636),
+  ('expr -> expr PLUS expr','expr',3,'p_expr_arithmetic','yacc.py',640),
+  ('expr -> expr MINUS expr','expr',3,'p_expr_arithmetic','yacc.py',641),
+  ('expr -> expr TIMES expr','expr',3,'p_expr_arithmetic','yacc.py',642),
+  ('expr -> expr DIVIDE expr','expr',3,'p_expr_arithmetic','yacc.py',643),
+  ('expr -> expr MOD expr','expr',3,'p_expr_arithmetic','yacc.py',644),
+  ('expr -> NOT expr','expr',2,'p_expr_not','yacc.py',649),
+  ('expr -> MINUS expr','expr',2,'p_expr_not','yacc.py',650),
+  ('expr -> LNOT expr','expr',2,'p_expr_not','yacc.py',651),
+  ('expr -> expr AND expr','expr',3,'p_expr_logical','yacc.py',656),
+  ('expr -> expr OR expr','expr',3,'p_expr_logical','yacc.py',657),
+  ('expr -> expr XOR expr','expr',3,'p_expr_logical','yacc.py',658),
+  ('expr -> expr LAND expr','expr',3,'p_expr_logical','yacc.py',659),
+  ('expr -> expr LOR expr','expr',3,'p_expr_logical','yacc.py',660),
+  ('expr -> expr LSHIFT expr','expr',3,'p_expr_shift','yacc.py',667),
+  ('expr -> expr RSHIFT expr','expr',3,'p_expr_shift','yacc.py',668),
+  ('expr -> const','expr',1,'p_expr_const_varref','yacc.py',673),
+  ('expr -> varref','expr',1,'p_expr_const_varref','yacc.py',674),
+  ('expr -> varref RCV LBRACKET rargs RBRACKET','expr',5,'p_expr_varref','yacc.py',679),
+  ('expr -> varref R_RCV LBRACKET rargs RBRACKET','expr',5,'p_expr_varref','yacc.py',680),
+  ('expr -> LPAREN expr ARROW expr COLON expr RPAREN','expr',7,'p_expr_other','yacc.py',686),
+  ('expr -> LEN LPAREN varref RPAREN','expr',4,'p_expr_other','yacc.py',687),
+  ('expr -> ENABLED LPAREN expr RPAREN','expr',4,'p_expr_other','yacc.py',688),
+  ('expr -> GET_P LPAREN expr RPAREN','expr',4,'p_expr_other','yacc.py',689),
+  ('expr -> RUN aname LPAREN args RPAREN opt_priority','expr',6,'p_expr_run','yacc.py',695),
+  ('expr -> TIMEOUT','expr',1,'p_expr_other_2','yacc.py',699),
+  ('expr -> NONPROGRESS','expr',1,'p_expr_other_2','yacc.py',700),
+  ('expr -> PC_VAL LPAREN expr RPAREN','expr',4,'p_expr_other_2','yacc.py',701),
+  ('expr -> NAME AT NAME','expr',3,'p_expr_remote_ref_proctype_pc','yacc.py',706),
+  ('expr -> NAME LBRACKET expr RBRACKET AT NAME','expr',6,'p_expr_remote_ref_pid_pc','yacc.py',711),
+  ('expr -> NAME LBRACKET expr RBRACKET COLON pfld','expr',6,'p_expr_remote_ref_var','yacc.py',715),
+  ('expr -> expr EQ expr','expr',3,'p_expr_comparator','yacc.py',720),
+  ('expr -> expr NE expr','expr',3,'p_expr_comparator','yacc.py',721),
+  ('expr -> expr LT expr','expr',3,'p_expr_comparator','yacc.py',722),
+  ('expr -> expr LE expr','expr',3,'p_expr_comparator','yacc.py',723),
+  ('expr -> expr GT expr','expr',3,'p_expr_comparator','yacc.py',724),
+  ('expr -> expr GE expr','expr',3,'p_expr_comparator','yacc.py',725),
+  ('expr -> expr UNTIL expr','expr',3,'p_binary_ltl_expr','yacc.py',730),
+  ('expr -> expr WEAK_UNTIL expr','expr',3,'p_binary_ltl_expr','yacc.py',731),
+  ('expr -> expr RELEASE expr','expr',3,'p_binary_ltl_expr','yacc.py',732),
+  ('expr -> expr IMPLIES expr','expr',3,'p_binary_ltl_expr','yacc.py',733),
+  ('expr -> expr EQUIV expr','expr',3,'p_binary_ltl_expr','yacc.py',734),
+  ('expr -> NEXT expr','expr',2,'p_unary_ltl_expr','yacc.py',739),
+  ('expr -> ALWAYS expr','expr',2,'p_unary_ltl_expr','yacc.py',740),
+  ('expr -> EVENTUALLY expr','expr',2,'p_unary_ltl_expr','yacc.py',741),
+  ('const_expr -> const','const_expr',1,'p_const_expr_const','yacc.py',749),
+  ('const_expr -> MINUS const_expr','const_expr',2,'p_const_expr_unary','yacc.py',753),
+  ('const_expr -> const_expr PLUS const_expr','const_expr',3,'p_const_expr_binary','yacc.py',757),
+  ('const_expr -> const_expr MINUS const_expr','const_expr',3,'p_const_expr_binary','yacc.py',758),
+  ('const_expr -> const_expr TIMES const_expr','const_expr',3,'p_const_expr_binary','yacc.py',759),
+  ('const_expr -> const_expr DIVIDE const_expr','const_expr',3,'p_const_expr_binary','yacc.py',760),
+  ('const_expr -> const_expr MOD const_expr','const_expr',3,'p_const_expr_binary','yacc.py',761),
+  ('const_expr -> LPAREN const_expr RPAREN','const_expr',3,'p_const_expr_paren','yacc.py',766),
+  ('const -> boolean','const',1,'p_const','yacc.py',770),
+  ('const -> number','const',1,'p_const','yacc.py',771),
+  ('boolean -> TRUE','boolean',1,'p_bool','yacc.py',777),
+  ('boolean -> FALSE','boolean',1,'p_bool','yacc.py',778),
+  ('number -> INTEGER','number',1,'p_number','yacc.py',783),
+  ('two_args -> expr COMMA expr','two_args',3,'p_two_args','yacc.py',790),
+  ('args -> arg','args',1,'p_args','yacc.py',793),
+  ('prargs -> COMMA arg','prargs',2,'p_prargs','yacc.py',797),
+  ('prargs -> empty','prargs',1,'p_prargs_empty','yacc.py',801),
+  ('args -> empty','args',1,'p_args_empty','yacc.py',804),
+  ('margs -> arg','margs',1,'p_margs','yacc.py',807),
+  ('margs -> expr LPAREN arg RPAREN','margs',4,'p_margs','yacc.py',808),
+  ('arg -> expr','arg',1,'p_arg','yacc.py',812),
+  ('arg -> expr COMMA arg','arg',3,'p_arg','yacc.py',813),
+  ('rarg -> varref','rarg',1,'p_rarg','yacc.py',819),
+  ('rarg -> EVAL LPAREN expr RPAREN','rarg',4,'p_rarg','yacc.py',820),
+  ('rargs -> rarg','rargs',1,'p_rargs','yacc.py',825),
+  ('rargs -> rarg COMMA rargs','rargs',3,'p_rargs','yacc.py',826),
+  ('rargs -> rarg LPAREN rargs RPAREN','rargs',4,'p_rargs','yacc.py',827),
+  ('rargs -> LPAREN rargs RPAREN','rargs',3,'p_rargs','yacc.py',828),
+  ('proctype -> PROCTYPE','proctype',1,'p_proctype','yacc.py',832),
+  ('proctype -> D_PROCTYPE','proctype',1,'p_proctype','yacc.py',833),
+  ('aname -> NAME','aname',1,'p_aname','yacc.py',842),
+  ('optname -> NAME','optname',1,'p_optname','yacc.py',847),
+  ('optname -> empty','optname',1,'p_optname_empty','yacc.py',851),
+  ('os -> empty','os',1,'p_os','yacc.py',855),
+  ('os -> semi','os',1,'p_os','yacc.py',856),
+  ('msemi -> semi','msemi',1,'p_msemi','yacc.py',862),
+  ('msemi -> msemi semi','msemi',2,'p_msemi','yacc.py',863),
+  ('semi -> SEMI','semi',1,'p_semi','yacc.py',868),
+  ('semi -> ARROW','semi',1,'p_semi','yacc.py',869),
+  ('asgn -> EQUALS','asgn',1,'p_asgn','yacc.py',874),
+  ('asgn -> empty','asgn',1,'p_asgn','yacc.py',875),
+  ('vis -> HIDDEN','vis',1,'p_visible','yacc.py',880),
+  ('vis -> SHOW','vis',1,'p_visible','yacc.py',881),
+  ('vis -> ISLOCAL','vis',1,'p_visible','yacc.py',882),
+  ('empty -> <empty>','empty',0,'p_empty','yacc.py',887),
 ]
```

### Comparing `promela-0.0.3/promela/yacc.py` & `promela-0.0.4/promela/yacc.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,74 +2,75 @@
 
 
 References
 ==========
 
 Holzmann G.J., The SPIN Model Checker,
     Addison-Wesley, 2004, pp. 365--368
-    http://spinroot.com/spin/Man/Quick.html
+    <https://spinroot.com/spin/Man/Quick.html>
 """
-from __future__ import absolute_import
-from __future__ import division
 import logging
 import os
 import subprocess
 import warnings
+
 import ply.yacc
 # inline
 #
 # import promela.ast as promela_ast
 # from promela import lex
 
 
 TABMODULE = 'promela.promela_parsetab'
 logger = logging.getLogger(__name__)
 
 
-class Parser(object):
+class Parser:
     """Production rules for Promela parser."""
 
-    logger = logger
-    tabmodule = TABMODULE
-    start = 'program'
-    # http://spinroot.com/spin/Man/operators.html
-    # spin.y
-    # lowest to highest
-    precedence = (
-        ('right', 'EQUALS'),
-        ('left', 'TX2', 'RCV', 'R_RCV'),
-        ('left', 'IMPLIES', 'EQUIV'),
-        ('left', 'LOR'),
-        ('left', 'LAND'),
-        ('left', 'ALWAYS', 'EVENTUALLY'),
-        ('left', 'UNTIL', 'WEAK_UNTIL', 'RELEASE'),
-        ('right', 'NEXT'),
-        ('left', 'OR'),
-        ('left', 'XOR'),
-        ('left', 'AND'),
-        ('left', 'EQ', 'NE'),
-        ('left', 'LT', 'LE', 'GT', 'GE'),
-        ('left', 'LSHIFT', 'RSHIFT'),
-        ('left', 'PLUS', 'MINUS'),
-        ('left', 'TIMES', 'DIVIDE', 'MOD'),
-        ('left', 'INCR', 'DECR'),
-        ('right', 'LNOT', 'NOT', 'UMINUS', 'NEG'),  # LNOT is also SND
-        ('left', 'DOT'),
-        ('left', 'LPAREN', 'RPAREN', 'LBRACKET', 'RBRACKET'))
-
     def __init__(self, ast=None, lexer=None):
         if ast is None:
             import promela.ast as ast
+            self.ast = ast
+        else:
+            self.ast = ast
         if lexer is None:
             from promela import lex
-            lexer = lex.Lexer()
-        self.lexer = lexer
-        self.ast = ast
+            self.lexer = lex.Lexer()
+        else:
+            self.lexer = lexer
+        self.logger = logger
+        self.tabmodule = TABMODULE
+        self.start = 'program'
+        # <https://spinroot.com/spin/Man/operators.html>
+        # `spin.y`
+        # lowest to highest
+        self.precedence = (
+            ('right', 'EQUALS'),
+            ('left', 'TX2', 'RCV', 'R_RCV'),
+            ('left', 'IMPLIES', 'EQUIV'),
+            ('left', 'LOR'),
+            ('left', 'LAND'),
+            ('left', 'ALWAYS', 'EVENTUALLY'),
+            ('left', 'UNTIL', 'WEAK_UNTIL', 'RELEASE'),
+            ('right', 'NEXT'),
+            ('left', 'OR'),
+            ('left', 'XOR'),
+            ('left', 'AND'),
+            ('left', 'EQ', 'NE'),
+            ('left', 'LT', 'LE', 'GT', 'GE'),
+            ('left', 'LSHIFT', 'RSHIFT'),
+            ('left', 'PLUS', 'MINUS'),
+            ('left', 'TIMES', 'DIVIDE', 'MOD'),
+            ('left', 'INCR', 'DECR'),
+            ('right', 'LNOT', 'NOT', 'UMINUS', 'NEG'),  # LNOT is also SND
+            ('left', 'DOT'),
+            ('left', 'LPAREN', 'RPAREN', 'LBRACKET', 'RBRACKET'))
         self.tokens = self.lexer.tokens
-        self.build()
+        self.parser = None
 
     def build(self, tabmodule=None, outputdir='', write_tables=False,
               debug=False, debuglog=None, errorlog=None):
         """Build parser using `ply.yacc`.
 
         Default table module is `self.tabmodule`.
         Module logger used as default debug logger.
@@ -88,14 +89,16 @@
             write_tables=write_tables,
             debug=debug,
             debuglog=debuglog,
             errorlog=errorlog)
 
     def parse(self, promela):
         """Parse string of Promela code."""
+        if self.parser is None:
+            self.build()
         s = cpp(promela)
         program = self.parser.parse(
             s, lexer=self.lexer.lexer, debug=self.logger)
         return program
 
     def _iter(self, p):
         if p[2] is not None:
@@ -247,15 +250,15 @@
     # message type declaration
     def p_one_decl_mtype_vis(self, p):
         """one_decl : vis MTYPE asgn LBRACE name_list RBRACE"""
         p[0] = self.ast.MessageType(p[5], visible=p[1])
 
     def p_one_decl_mtype(self, p):
         """one_decl : MTYPE asgn LBRACE name_list RBRACE"""
-        p[0] = self.ast.MessageType(p[3])
+        p[0] = self.ast.MessageType(p[4])
 
     def p_name_list_iter(self, p):
         """name_list : name_list COMMA NAME"""
         p[1].append(p[3])
         p[0] = p[1]
 
     def p_name_list_end(self, p):
@@ -421,15 +424,15 @@
                 | stmnt
         """
         p[0] = p[1]
 
     def p_step_labeled(self, p):
         """step : NAME COLON one_decl"""
         raise Exception(
-            'label preceding declaration: {s}'.format(s=p[3]))
+            f'label preceding declaration: {p[3]}')
 
     def p_step_3(self, p):
         """step : NAME COLON XR
                 | NAME COLON XS
         """
         raise Exception(
             'label preceding xr/xs claim')
@@ -682,15 +685,15 @@
     def p_expr_other(self, p):
         """expr : LPAREN expr ARROW expr COLON expr RPAREN
                 | LEN LPAREN varref RPAREN
                 | ENABLED LPAREN expr RPAREN
                 | GET_P LPAREN expr RPAREN
         """
         p[0] = p[1]
-        warnings.warn('"{s}" not implemented'.format(s=p[1]))
+        warnings.warn(f'"{p[1]}" not implemented')
 
     def p_expr_run(self, p):
         """expr : RUN aname LPAREN args RPAREN opt_priority"""
         p[0] = self.ast.Run(p[2], p[4], p[6])
 
     def p_expr_other_2(self, p):
         """expr : TIMEOUT
@@ -880,34 +883,39 @@
         """
         p[0] = {'visible': p[1]}
 
     def p_empty(self, p):
         """empty : """
 
     def p_error(self, p):
-        raise Exception('syntax error at: {p}'.format(p=p))
+        raise Exception(f'syntax error at: {p}')
 
 
 def cpp(s):
-    """Call the C{C} preprocessor with input C{s}."""
+    """Call the C preprocessor with input `s`."""
     try:
         p = subprocess.Popen(['cpp', '-E', '-x', 'c'],
                              stdin=subprocess.PIPE,
                              stdout=subprocess.PIPE,
                              stderr=subprocess.PIPE,
                              universal_newlines=True)
     except OSError as e:
         if e.errno == os.errno.ENOENT:
             raise Exception('C preprocessor (cpp) not found in path.')
         else:
             raise
     logger.debug('cpp input:\n' + s)
     stdout, stderr = p.communicate(s)
-    logger.debug('cpp returned: {c}'.format(c=p.returncode))
-    logger.debug('cpp stdout:\n {out}'.format(out=stdout))
+    if p.returncode != 0:
+        raise RuntimeError(
+            p.returncode,
+            stderr,
+            stdout)
+    logger.debug(f'cpp returned: {p.returncode}')
+    logger.debug(f'cpp stdout:\n {stdout}')
     return stdout
 
 
 def rebuild_table(parser, tabmodule):
     # log details to file
     h = logging.FileHandler('log.txt', mode='w')
     debuglog = logging.getLogger()
@@ -917,26 +925,26 @@
     outputdir = './'
     # rm table files to force rebuild to get debug output
     tablepy = tabmodule + '.py'
     tablepyc = tabmodule + '.pyc'
     try:
         os.remove(tablepy)
     except:
-        print('no "{t}" found'.format(t=tablepy))
+        print(f'no "{tablepy}" found')
     try:
         os.remove(tablepyc)
     except:
-        print('no "{t}" found'.format(t=tablepyc))
+        print(f'no "{tablepyc}" found')
     parser.build(tabmodule, outputdir=outputdir,
                  write_tables=True, debug=True,
                  debuglog=debuglog)
 
 
 if __name__ == '__main__':
-    rebuild_table(Parser(), TABMODULE.split('.')[-1])
+    rebuild_table(Parser(), TABMODULE.rpartition('.')[-1])
 
 
 # TODO
 #
 # expr << expr
 # expr >> expr
 # (expr -> expr : expr)
```

### Comparing `promela-0.0.3/promela.egg-info/PKG-INFO` & `promela-0.0.4/promela.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: promela
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parser and abstract syntax tree for the Promela modeling language.
 Home-page: https://github.com/johnyf/promela
 Author: Ioannis Filippidis
 Author-email: jfilippidis@gmail.com
 License: BSD
-Description: [![Build Status][build_img]][travis]
-        [![Coverage Status][coverage]][coveralls]
-        
-        
-        About
-        =====
-        
-        A parser for the [Promela modeling language](https://en.wikipedia.org/wiki/Promela).
-        [PLY](https://pypi.python.org/pypi/ply/3.4) (Python `lex`-`yacc`) is used to generate the parser.
-        Classes for a Promela abstract tree are included and used for representing the result of parsing.
-        A short tutorial can be found in the file [`doc.md`](
-            https://github.com/johnyf/promela/blob/master/doc.md).
-        To install:
-        
-        ```
-        pip install promela
-        ```
-        
-        
-        License
-        =======
-        [BSD-3](http://opensource.org/licenses/BSD-3-Clause), see `LICENSE` file.
-        
-        
-        [build_img]: https://travis-ci.org/johnyf/promela.svg?branch=master
-        [travis]: https://travis-ci.org/johnyf/promela
-        [coverage]: https://coveralls.io/repos/johnyf/promela/badge.svg?branch=master
-        [coveralls]: https://coveralls.io/r/johnyf/promela?branch=master
-        
+Project-URL: Bug Tracker, https://github.com/johnyf/promela/issues
+Project-URL: Documentation, https://github.com/johnyf/promela/blob/main/doc.md
 Keywords: promela,parser,syntax tree,ply,lex,yacc
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: networkx>=2.0
+Requires-Dist: ply<=3.10,>=3.4
+
+[![Build Status][build_img]][ci]
+
+
+About
+=====
+
+A parser for the [Promela modeling language](https://en.wikipedia.org/wiki/Promela).
+[PLY](https://pypi.org/project/ply/3.4/) (Python `lex`-`yacc`) is used to
+generate the parser. Classes for a Promela abstract tree are included and used
+for representing the result of parsing.
+
+A short tutorial can be found in the file [`doc.md`](
+    https://github.com/johnyf/promela/blob/main/doc.md).
+To install:
+
+```
+pip install promela
+```
+
+
+License
+=======
+
+[3-clause BSD](https://opensource.org/licenses/BSD-3-Clause),
+see the file `LICENSE`.
+
+
+[build_img]: https://github.com/johnyf/promela/actions/workflows/main.yml/badge.svg?branch=main
+[ci]: https://github.com/johnyf/promela/actions
```

### Comparing `promela-0.0.3/setup.py` & `promela-0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,89 @@
-from setuptools import setup
+"""Installation script."""
+import setuptools
 # inline:
 # from promela import yacc
 
 
-description = (
+DESCRIPTION = (
     'Parser and abstract syntax tree for the Promela modeling language.')
 README = 'README.md'
+PROJECT_URLS = {
+    'Bug Tracker':
+        'https://github.com/johnyf/promela/issues',
+    'Documentation':
+        'https://github.com/johnyf/promela/blob/main/doc.md',}
 VERSION_FILE = 'promela/_version.py'
 MAJOR = 0
 MINOR = 0
-MICRO = 3
-version = '{major}.{minor}.{micro}'.format(
-    major=MAJOR, minor=MINOR, micro=MICRO)
-s = (
+MICRO = 4
+VERSION = f'{MAJOR}.{MINOR}.{MICRO}'
+VERSION_FILE_TEXT = (
     '# This file was generated from setup.py\n'
-    "version = '{version}'\n").format(version=version)
-install_requires = [
+    f"version = '{VERSION}'\n")
+PYTHON_REQUIRES = '>=3.9'
+INSTALL_REQUIRES = [
     'networkx >= 2.0',
-    'ply >= 3.4, <= 3.10',
-    'pydot >= 1.1.0']
-classifiers = [
+    'ply >= 3.4, <= 3.10']
+CLASSIFIERS = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3 :: Only',
     'Topic :: Scientific/Engineering']
-keywords = [
+KEYWORDS = [
     'promela', 'parser', 'syntax tree', 'ply', 'lex', 'yacc']
 
 
-def build_parser_table():
+def _build_parser_table():
+    if not _ply_is_installed():
+        return
     from promela import yacc
-    tabmodule = yacc.TABMODULE.split('.')[-1]
+    tabmodule = yacc.TABMODULE.rpartition('.')[-1]
     outputdir = 'promela/'
     parser = yacc.Parser()
-    parser.build(tabmodule, outputdir=outputdir, write_tables=True)
+    parser.build(
+        tabmodule,
+        outputdir=outputdir,
+        write_tables=True)
 
 
-if __name__ == '__main__':
-    with open(VERSION_FILE, 'w') as f:
-        f.write(s)
+def _ply_is_installed():
     try:
-        build_parser_table()
+        import ply
     except ImportError:
         print('WARNING: `promela` could not cache parser tables '
               '(ignore this if running only for "egg_info").')
-    setup(
+        return False
+    return True
+
+
+def run_setup():
+    with open(VERSION_FILE, 'w') as f:
+        f.write(VERSION_FILE_TEXT)
+    _build_parser_table()
+    with open(README) as f:
+        long_description = f.read()
+    setuptools.setup(
         name='promela',
-        version=version,
-        description=description,
-        long_description=open(README).read(),
+        version=VERSION,
+        description=DESCRIPTION,
+        long_description=long_description,
         long_description_content_type='text/markdown',
         author='Ioannis Filippidis',
         author_email='jfilippidis@gmail.com',
         url='https://github.com/johnyf/promela',
+        project_urls=PROJECT_URLS,
         license='BSD',
-        install_requires=install_requires,
-        tests_require=['nose'],
+        python_requires=PYTHON_REQUIRES,
+        install_requires=INSTALL_REQUIRES,
+        tests_require=['pytest'],
         packages=['promela'],
         package_dir={'promela': 'promela'},
-        classifiers=classifiers,
-        keywords=keywords)
+        classifiers=CLASSIFIERS,
+        keywords=KEYWORDS)
+
+
+if __name__ == '__main__':
+    run_setup()
```

### Comparing `promela-0.0.3/tests/yacc_test.py` & `promela-0.0.4/tests/yacc_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
+
 import networkx as nx
 import networkx.algorithms.isomorphism as iso
-from nose.tools import assert_raises
+from pytest import raises
 from promela import ast, yacc
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel('WARNING')
 log = logging.getLogger('promela.yacc')
 log.setLevel(logging.ERROR)
@@ -341,15 +342,15 @@
     proctype p(){
         do
         :: S0: x = 1;
         od
     }
     '''
     tree = parser.parse(s)
-    with assert_raises(Exception):
+    with raises(Exception):
         tree[0].to_pg()
 
 
 def goto_pg_test():
     s = '''
     proctype p(){
         bit x;
@@ -428,15 +429,15 @@
     s = '''
     proctype p(){
         S0: goto S1;
         S1: goto S0
     }
     '''
     tree = parser.parse(s)
-    with assert_raises(AssertionError):
+    with raises(AssertionError):
         tree[0].to_pg()
 
 
 def break_pg_test():
     s = '''
     proctype p(){
         bit x;
@@ -658,15 +659,15 @@
             fi
         :: else
         od
     }
     '''
     # syntactic else = Promela language definition
     (proc,) = parser.parse(s)
-    with assert_raises(AssertionError):
+    with raises(AssertionError):
         proc.to_pg()
     # different from Promela language definition
     g = proc.to_pg(syntactic_else=True)
     active_else = 0
     off_else = 0
     for u, v, d in g.edges(data=True):
         stmt = d['stmt']
```

