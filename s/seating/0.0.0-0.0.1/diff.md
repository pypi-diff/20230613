# Comparing `tmp/seating-0.0.0.tar.gz` & `tmp/seating-0.0.1.tar.gz`

## Comparing `seating-0.0.0.tar` & `seating-0.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 seating-0.0.0/docs/index.html
--rw-r--r--   0        0        0    28186 2020-02-02 00:00:00.000000 seating-0.0.0/docs/search.js
--rw-r--r--   0        0        0    34048 2020-02-02 00:00:00.000000 seating-0.0.0/docs/seating.html
--rw-r--r--   0        0        0   160282 2020-02-02 00:00:00.000000 seating-0.0.0/docs/seating/seating.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 seating-0.0.0/src/seating/__init__.py
--rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 seating-0.0.0/src/seating/seating.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 seating-0.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 seating-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 seating-0.0.0/README.md
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 seating-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 seating-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 seating-0.0.1/docs/index.html
+-rw-r--r--   0        0        0    28083 2020-02-02 00:00:00.000000 seating-0.0.1/docs/search.js
+-rw-r--r--   0        0        0    34048 2020-02-02 00:00:00.000000 seating-0.0.1/docs/seating.html
+-rw-r--r--   0        0        0   171907 2020-02-02 00:00:00.000000 seating-0.0.1/docs/seating/seating.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 seating-0.0.1/src/seating/__init__.py
+-rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 seating-0.0.1/src/seating/seating.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 seating-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 seating-0.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 seating-0.0.1/README.md
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 seating-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 seating-0.0.1/PKG-INFO
```

### Comparing `seating-0.0.0/docs/search.js` & `seating-0.0.1/docs/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -697,64 +697,64 @@
         "modulename": "seating.seating",
         "qualname": "get_seat_sections",
         "kind": "function",
         "doc": "<p>Return a list of line number pairs for content between <code># Seat</code> comments in <code>source</code>.</p>\n\n<p>If <code>source</code> has no <code># Seat</code> comments, a list with one tuple will be returned: <code>[(1, number_of_lines_in_source)]</code></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">source</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">,</span> <span class=\"nb\">int</span><span class=\"p\">]]</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "seating.seating.Order",
+        "fullname": "seating.seating.Seats",
         "modulename": "seating.seating",
-        "qualname": "Order",
+        "qualname": "Seats",
         "kind": "class",
         "doc": "<p></p>\n"
     }, {
-        "fullname": "seating.seating.Order.__init__",
+        "fullname": "seating.seating.Seats.__init__",
         "modulename": "seating.seating",
-        "qualname": "Order.__init__",
+        "qualname": "Seats.__init__",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">()</span>"
     }, {
-        "fullname": "seating.seating.Order.sort_nodes_by_name",
+        "fullname": "seating.seating.Seats.sort_nodes_by_name",
         "modulename": "seating.seating",
-        "qualname": "Order.sort_nodes_by_name",
+        "qualname": "Seats.sort_nodes_by_name",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">nodes</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "seating.seating.Order.sort_dunders",
+        "fullname": "seating.seating.Seats.sort_dunders",
         "modulename": "seating.seating",
-        "qualname": "Order.sort_dunders",
+        "qualname": "Seats.sort_dunders",
         "kind": "function",
         "doc": "<p>Sort <code>dunders</code> alphabetically, except <code>__init__</code> is placed at the front, if it exists.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">dunders</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "seating.seating.Order.sort_assigns",
+        "fullname": "seating.seating.Seats.sort_assigns",
         "modulename": "seating.seating",
-        "qualname": "Order.sort_assigns",
+        "qualname": "Seats.sort_assigns",
         "kind": "function",
         "doc": "<p>Sort assignment statments.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">assigns</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "seating.seating.Order.sort",
+        "fullname": "seating.seating.Seats.sort",
         "modulename": "seating.seating",
-        "qualname": "Order.sort",
+        "qualname": "Seats.sort",
         "kind": "function",
         "doc": "<p>Sort and return members as a single list.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "seating.seating.seat",
         "modulename": "seating.seating",
         "qualname": "seat",
         "kind": "function",
-        "doc": "<p>Sort the contents of classes in <code>source</code>, where <code>source</code> is parsable Python code.\nAnything not inside a class will be untouched.</p>\n\n<p>The modified <code>source</code> will be returned.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<ul>\n<li><p><code>start_line</code>: Only sort contents after this line.</p></li>\n<li><p><code>stop_line</code>: Only sort contents before this line.</p></li>\n</ul>\n\n<p>If you have class contents that are grouped a certain way and you want the groups individually sorted\nso that the grouping is maintained, you can use <code># Seat</code> to demarcate the groups.</p>\n\n<p>Note: Comments that are in a class body, but not in a function will remain at the same line.</p>\n\n<p>i.e. if the source is:</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">class</span> <span class=\"nc\">MyClass</span><span class=\"p\">():</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">arbitrary</span> <span class=\"n\">lines</span> <span class=\"n\">of</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"c1\"># Seat</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">more</span> <span class=\"n\">arbitrary</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"c1\"># Seat</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">yet</span> <span class=\"n\">more</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n</code></pre>\n</div>\n\n<p>Then the three sets of code in brackets will be sorted independently from one another\n(assuming no values are given for <code>start_line</code> or <code>stop_line</code>).</p>\n\n<h4 id=\"sorting-and-priority\">:Sorting and Priority:</h4>\n\n<ul>\n<li>Class variables declared in class body outside of a function</li>\n<li>Dunder methods</li>\n<li>Functions decorated with <code>property</code> or corresponding <code>.setter</code> and <code>.deleter</code> methods</li>\n<li>Class functions</li>\n</ul>\n\n<p>Each of these groups will be sorted alphabetically with respect to themselves.</p>\n\n<p>The only exception is for dunder methods.\nThey will be sorted alphabetically except that <code>__init__</code> will be first.</p>\n",
+        "doc": "<p>Sort the contents of classes in <code>source</code>, where <code>source</code> is parsable Python code.\nAnything not inside a class will be untouched.</p>\n\n<p>The modified <code>source</code> will be returned.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<ul>\n<li><p><code>start_line</code>: Only sort contents after this line.</p></li>\n<li><p><code>stop_line</code>: Only sort contents before this line.</p></li>\n</ul>\n\n<p>If you have class contents that are grouped a certain way and you want the groups individually sorted\nso that the grouping is maintained, you can use <code># Seat</code> to demarcate the groups.</p>\n\n<p>i.e. if the source is:</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">class</span> <span class=\"nc\">MyClass</span><span class=\"p\">():</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">arbitrary</span> <span class=\"n\">lines</span> <span class=\"n\">of</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"c1\"># Seat</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">more</span> <span class=\"n\">arbitrary</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"c1\"># Seat</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">yet</span> <span class=\"n\">more</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n</code></pre>\n</div>\n\n<p>Then the three sets of code in brackets will be sorted independently from one another\n(assuming no values are given for <code>start_line</code> or <code>stop_line</code>).</p>\n\n<h4 id=\"sorting-and-priority\">:Sorting and Priority:</h4>\n\n<ul>\n<li>Class variables declared in class body outside of a function</li>\n<li>Dunder methods</li>\n<li>Functions decorated with <code>property</code> or corresponding <code>.setter</code> and <code>.deleter</code> methods</li>\n<li>Class functions</li>\n</ul>\n\n<p>Each of these groups will be sorted alphabetically with respect to themselves.</p>\n\n<p>The only exception is for dunder methods.\nThey will be sorted alphabetically except that <code>__init__</code> will be first.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">source</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">start_line</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">stop_line</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "seating.seating.get_args",
         "modulename": "seating.seating",
         "qualname": "get_args",
         "kind": "function",
```

### Comparing `seating-0.0.0/docs/seating.html` & `seating-0.0.1/docs/seating.html`

 * *Files identical despite different names*

### Comparing `seating-0.0.0/docs/seating/seating.html` & `seating-0.0.1/docs/seating/seating.html`

 * *Files 3% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
                     <a class="function" href="#get_seat_sections">get_seat_sections</a>
             </li>
             <li>
-                    <a class="class" href="#Order">Order</a>
+                    <a class="class" href="#Seats">Seats</a>
                             <ul class="memberlist">
                         <li>
-                                <a class="function" href="#Order.__init__">Order</a>
+                                <a class="function" href="#Seats.__init__">Seats</a>
                         </li>
                         <li>
-                                <a class="function" href="#Order.sort_nodes_by_name">sort_nodes_by_name</a>
+                                <a class="function" href="#Seats.sort_nodes_by_name">sort_nodes_by_name</a>
                         </li>
                         <li>
-                                <a class="function" href="#Order.sort_dunders">sort_dunders</a>
+                                <a class="function" href="#Seats.sort_dunders">sort_dunders</a>
                         </li>
                         <li>
-                                <a class="function" href="#Order.sort_assigns">sort_assigns</a>
+                                <a class="function" href="#Seats.sort_assigns">sort_assigns</a>
                         </li>
                         <li>
-                                <a class="function" href="#Order.sort">sort</a>
+                                <a class="function" href="#Seats.sort">sort</a>
                         </li>
                 </ul>
 
             </li>
             <li>
                     <a class="function" href="#seat">seat</a>
             </li>
@@ -107,203 +107,222 @@
 </span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>                <span class="k">else</span><span class="p">:</span>
 </span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>                    <span class="n">sections</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">previous_endline</span><span class="p">()</span> <span class="o">+</span> <span class="mi">1</span><span class="p">,</span> <span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">))</span>
 </span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>        <span class="n">sections</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">previous_endline</span><span class="p">()</span> <span class="o">+</span> <span class="mi">1</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">lines</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">))</span>
 </span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>        <span class="k">return</span> <span class="n">sections</span>
 </span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="k">return</span> <span class="p">[(</span><span class="mi">1</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span><span class="p">)]</span>
 </span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
 </span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="k">class</span> <span class="nc">Order</span><span class="p">:</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="k">class</span> <span class="nc">Seats</span><span class="p">:</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">before</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">after</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">seats</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="k">def</span> <span class="nf">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">nodes</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">nodes</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">node</span><span class="p">:</span> <span class="n">node</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="k">def</span> <span class="nf">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dunders</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="sd">&quot;&quot;&quot;Sort `dunders` alphabetically, except `__init__` is placed at the front, if it exists.&quot;&quot;&quot;</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="n">dunders</span><span class="p">)</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="n">init</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">dunder</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">dunders</span><span class="p">):</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>            <span class="k">if</span> <span class="n">dunder</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>                <span class="n">init</span> <span class="o">=</span> <span class="n">dunders</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>                <span class="k">break</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="k">if</span> <span class="n">init</span><span class="p">:</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>            <span class="n">dunders</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">init</span><span class="p">)</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="k">return</span> <span class="n">dunders</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="k">def</span> <span class="nf">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">assigns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="sd">&quot;&quot;&quot;Sort assignment statments.&quot;&quot;&quot;</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="k">def</span> <span class="nf">get_name</span><span class="p">(</span><span class="n">node</span><span class="p">:</span> <span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>            <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">node</span><span class="p">)</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>            <span class="k">if</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">:</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">targets</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">id</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">target</span><span class="o">.</span><span class="n">id</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">assigns</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="n">get_name</span><span class="p">)</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">sort</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="sd">&quot;&quot;&quot;Sort and return members as a single list.&quot;&quot;&quot;</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dunders</span><span class="p">)</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">functions</span><span class="p">)</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">properties</span><span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">assigns</span><span class="p">)</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="k">return</span> <span class="p">(</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">before</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">properties</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">functions</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">seats</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">after</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="p">)</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="c1"># These will be a list of tuples containing the node and the index it was found at</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="c1"># so they can be reinserted after sorting</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">expressions</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">comments</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">def</span> <span class="nf">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">nodes</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">nodes</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">node</span><span class="p">:</span> <span class="n">node</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="k">def</span> <span class="nf">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dunders</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="sd">&quot;&quot;&quot;Sort `dunders` alphabetically, except `__init__` is placed at the front, if it exists.&quot;&quot;&quot;</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="n">dunders</span><span class="p">)</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">init</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">dunder</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">dunders</span><span class="p">):</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>            <span class="k">if</span> <span class="n">dunder</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>                <span class="n">init</span> <span class="o">=</span> <span class="n">dunders</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>                <span class="k">break</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="k">if</span> <span class="n">init</span><span class="p">:</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>            <span class="n">dunders</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">init</span><span class="p">)</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="k">return</span> <span class="n">dunders</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="k">def</span> <span class="nf">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">assigns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="sd">&quot;&quot;&quot;Sort assignment statments.&quot;&quot;&quot;</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="k">def</span> <span class="nf">get_name</span><span class="p">(</span><span class="n">node</span><span class="p">:</span> <span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>            <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">node</span><span class="p">)</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>            <span class="k">if</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">:</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">targets</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">id</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">target</span><span class="o">.</span><span class="n">id</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">assigns</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="n">get_name</span><span class="p">)</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">sort</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="sd">&quot;&quot;&quot;Sort and return members as a single list.&quot;&quot;&quot;</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dunders</span><span class="p">)</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">functions</span><span class="p">)</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">properties</span><span class="p">)</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">assigns</span><span class="p">)</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="n">body</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">before</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">properties</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">functions</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">seats</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">after</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="p">)</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="k">for</span> <span class="n">expression</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">expressions</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">comments</span><span class="p">:</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>            <span class="n">body</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">expression</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">expression</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="k">return</span> <span class="n">body</span>
 </span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">    The modified `source` will be returned.</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">    #### :params:</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">    The modified `source` will be returned.</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">    Note: Comments that are in a class body, but not in a function will remain at the same line.</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">    i.e. if the source is:</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">    #### :Sorting and Priority:</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">    i.e. if the source is:</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
 </span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">    * Dunder methods</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">    * Class functions</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">    #### :Sorting and Priority:</span>
 </span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">    The only exception is for dunder methods.</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">comments</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Order</span><span class="p">()</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>                <span class="k">for</span> <span class="n">child</span> <span class="ow">in</span> <span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">:</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>                    <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>                    <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>                    <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>                    <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                        <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>                        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>                            <span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                    <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                    <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>                    <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                        <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                            <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                            <span class="k">if</span> <span class="p">(</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                                <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                                <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="s2">&quot;property&quot;</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                            <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                                <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>                                <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>                            <span class="p">):</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                                <span class="k">break</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>                        <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="c1"># Put comments back in</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="k">for</span> <span class="n">comment</span> <span class="ow">in</span> <span class="n">comments</span><span class="p">:</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="n">source</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">comment</span><span class="o">.</span><span class="n">lineno</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="n">comment</span><span class="o">.</span><span class="n">col_offset</span><span class="si">}{</span><span class="n">comment</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="p">)</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    * Dunder methods</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">    * Class functions</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">    The only exception is for dunder methods.</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Seats</span><span class="p">()</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>                <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">child</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>                        <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                        <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>                        <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Expr</span><span class="p">:</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">expressions</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>                            <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>                            <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>                                <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>                                <span class="k">if</span> <span class="p">(</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>                                    <span class="ow">and</span> <span class="s2">&quot;property&quot;</span> <span class="ow">in</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                                <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                                    <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>                                <span class="p">):</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>                                    <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>                                    <span class="k">break</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>                            <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>                        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">child</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">))</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>                        <span class="k">raise</span> <span class="n">e</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="k">return</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
 </span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
 </span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="p">)</span>
 </span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="p">)</span>
 </span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="p">)</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="p">)</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="s2">&quot;--dump&quot;</span><span class="p">,</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Dump ast tree to file instead of doing anything else. </span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="s2">        For debugging purposes.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="p">)</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
 </span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">dump</span><span class="p">:</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_ast_dump.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>            <span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="p">)</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_seat_sections">
                             <input id="get_seat_sections-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -339,211 +358,225 @@
             <div class="docstring"><p>Return a list of line number pairs for content between <code># Seat</code> comments in <code>source</code>.</p>
 
 <p>If <code>source</code> has no <code># Seat</code> comments, a list with one tuple will be returned: <code>[(1, number_of_lines_in_source)]</code></p>
 </div>
 
 
                 </section>
-                <section id="Order">
-                            <input id="Order-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="Seats">
+                            <input id="Seats-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
             
     <span class="def">class</span>
-    <span class="name">Order</span>:
+    <span class="name">Seats</span>:
 
-                <label class="view-source-button" for="Order-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Seats-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Order"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Order-29"><a href="#Order-29"><span class="linenos">29</span></a><span class="k">class</span> <span class="nc">Order</span><span class="p">:</span>
-</span><span id="Order-30"><a href="#Order-30"><span class="linenos">30</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Order-31"><a href="#Order-31"><span class="linenos">31</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">before</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order-32"><a href="#Order-32"><span class="linenos">32</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order-33"><a href="#Order-33"><span class="linenos">33</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order-34"><a href="#Order-34"><span class="linenos">34</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order-35"><a href="#Order-35"><span class="linenos">35</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order-36"><a href="#Order-36"><span class="linenos">36</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">after</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order-37"><a href="#Order-37"><span class="linenos">37</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">seats</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order-38"><a href="#Order-38"><span class="linenos">38</span></a>
-</span><span id="Order-39"><a href="#Order-39"><span class="linenos">39</span></a>    <span class="k">def</span> <span class="nf">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">nodes</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order-40"><a href="#Order-40"><span class="linenos">40</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">nodes</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">node</span><span class="p">:</span> <span class="n">node</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="Order-41"><a href="#Order-41"><span class="linenos">41</span></a>
-</span><span id="Order-42"><a href="#Order-42"><span class="linenos">42</span></a>    <span class="k">def</span> <span class="nf">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dunders</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order-43"><a href="#Order-43"><span class="linenos">43</span></a>        <span class="sd">&quot;&quot;&quot;Sort `dunders` alphabetically, except `__init__` is placed at the front, if it exists.&quot;&quot;&quot;</span>
-</span><span id="Order-44"><a href="#Order-44"><span class="linenos">44</span></a>        <span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="n">dunders</span><span class="p">)</span>
-</span><span id="Order-45"><a href="#Order-45"><span class="linenos">45</span></a>        <span class="n">init</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="Order-46"><a href="#Order-46"><span class="linenos">46</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">dunder</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">dunders</span><span class="p">):</span>
-</span><span id="Order-47"><a href="#Order-47"><span class="linenos">47</span></a>            <span class="k">if</span> <span class="n">dunder</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
-</span><span id="Order-48"><a href="#Order-48"><span class="linenos">48</span></a>                <span class="n">init</span> <span class="o">=</span> <span class="n">dunders</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
-</span><span id="Order-49"><a href="#Order-49"><span class="linenos">49</span></a>                <span class="k">break</span>
-</span><span id="Order-50"><a href="#Order-50"><span class="linenos">50</span></a>        <span class="k">if</span> <span class="n">init</span><span class="p">:</span>
-</span><span id="Order-51"><a href="#Order-51"><span class="linenos">51</span></a>            <span class="n">dunders</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">init</span><span class="p">)</span>
-</span><span id="Order-52"><a href="#Order-52"><span class="linenos">52</span></a>        <span class="k">return</span> <span class="n">dunders</span>
-</span><span id="Order-53"><a href="#Order-53"><span class="linenos">53</span></a>
-</span><span id="Order-54"><a href="#Order-54"><span class="linenos">54</span></a>    <span class="k">def</span> <span class="nf">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">assigns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order-55"><a href="#Order-55"><span class="linenos">55</span></a>        <span class="sd">&quot;&quot;&quot;Sort assignment statments.&quot;&quot;&quot;</span>
-</span><span id="Order-56"><a href="#Order-56"><span class="linenos">56</span></a>
-</span><span id="Order-57"><a href="#Order-57"><span class="linenos">57</span></a>        <span class="k">def</span> <span class="nf">get_name</span><span class="p">(</span><span class="n">node</span><span class="p">:</span> <span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Order-58"><a href="#Order-58"><span class="linenos">58</span></a>            <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">node</span><span class="p">)</span>
-</span><span id="Order-59"><a href="#Order-59"><span class="linenos">59</span></a>            <span class="k">if</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">:</span>
-</span><span id="Order-60"><a href="#Order-60"><span class="linenos">60</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">targets</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">id</span>
-</span><span id="Order-61"><a href="#Order-61"><span class="linenos">61</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Order-62"><a href="#Order-62"><span class="linenos">62</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">target</span><span class="o">.</span><span class="n">id</span>
-</span><span id="Order-63"><a href="#Order-63"><span class="linenos">63</span></a>
-</span><span id="Order-64"><a href="#Order-64"><span class="linenos">64</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">assigns</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="n">get_name</span><span class="p">)</span>
-</span><span id="Order-65"><a href="#Order-65"><span class="linenos">65</span></a>
-</span><span id="Order-66"><a href="#Order-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">sort</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order-67"><a href="#Order-67"><span class="linenos">67</span></a>        <span class="sd">&quot;&quot;&quot;Sort and return members as a single list.&quot;&quot;&quot;</span>
-</span><span id="Order-68"><a href="#Order-68"><span class="linenos">68</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dunders</span><span class="p">)</span>
-</span><span id="Order-69"><a href="#Order-69"><span class="linenos">69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">functions</span><span class="p">)</span>
-</span><span id="Order-70"><a href="#Order-70"><span class="linenos">70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">properties</span><span class="p">)</span>
-</span><span id="Order-71"><a href="#Order-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">assigns</span><span class="p">)</span>
-</span><span id="Order-72"><a href="#Order-72"><span class="linenos">72</span></a>        <span class="k">return</span> <span class="p">(</span>
-</span><span id="Order-73"><a href="#Order-73"><span class="linenos">73</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">before</span>
-</span><span id="Order-74"><a href="#Order-74"><span class="linenos">74</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span>
-</span><span id="Order-75"><a href="#Order-75"><span class="linenos">75</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span>
-</span><span id="Order-76"><a href="#Order-76"><span class="linenos">76</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">properties</span>
-</span><span id="Order-77"><a href="#Order-77"><span class="linenos">77</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">functions</span>
-</span><span id="Order-78"><a href="#Order-78"><span class="linenos">78</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">seats</span>
-</span><span id="Order-79"><a href="#Order-79"><span class="linenos">79</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">after</span>
-</span><span id="Order-80"><a href="#Order-80"><span class="linenos">80</span></a>        <span class="p">)</span>
+    <a class="headerlink" href="#Seats"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Seats-29"><a href="#Seats-29"><span class="linenos">29</span></a><span class="k">class</span> <span class="nc">Seats</span><span class="p">:</span>
+</span><span id="Seats-30"><a href="#Seats-30"><span class="linenos">30</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Seats-31"><a href="#Seats-31"><span class="linenos">31</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">before</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-32"><a href="#Seats-32"><span class="linenos">32</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-33"><a href="#Seats-33"><span class="linenos">33</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-34"><a href="#Seats-34"><span class="linenos">34</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-35"><a href="#Seats-35"><span class="linenos">35</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-36"><a href="#Seats-36"><span class="linenos">36</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">after</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-37"><a href="#Seats-37"><span class="linenos">37</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">seats</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-38"><a href="#Seats-38"><span class="linenos">38</span></a>        <span class="c1"># These will be a list of tuples containing the node and the index it was found at</span>
+</span><span id="Seats-39"><a href="#Seats-39"><span class="linenos">39</span></a>        <span class="c1"># so they can be reinserted after sorting</span>
+</span><span id="Seats-40"><a href="#Seats-40"><span class="linenos">40</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">expressions</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-41"><a href="#Seats-41"><span class="linenos">41</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">comments</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats-42"><a href="#Seats-42"><span class="linenos">42</span></a>
+</span><span id="Seats-43"><a href="#Seats-43"><span class="linenos">43</span></a>    <span class="k">def</span> <span class="nf">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">nodes</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats-44"><a href="#Seats-44"><span class="linenos">44</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">nodes</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">node</span><span class="p">:</span> <span class="n">node</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="Seats-45"><a href="#Seats-45"><span class="linenos">45</span></a>
+</span><span id="Seats-46"><a href="#Seats-46"><span class="linenos">46</span></a>    <span class="k">def</span> <span class="nf">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dunders</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats-47"><a href="#Seats-47"><span class="linenos">47</span></a>        <span class="sd">&quot;&quot;&quot;Sort `dunders` alphabetically, except `__init__` is placed at the front, if it exists.&quot;&quot;&quot;</span>
+</span><span id="Seats-48"><a href="#Seats-48"><span class="linenos">48</span></a>        <span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="n">dunders</span><span class="p">)</span>
+</span><span id="Seats-49"><a href="#Seats-49"><span class="linenos">49</span></a>        <span class="n">init</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="Seats-50"><a href="#Seats-50"><span class="linenos">50</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">dunder</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">dunders</span><span class="p">):</span>
+</span><span id="Seats-51"><a href="#Seats-51"><span class="linenos">51</span></a>            <span class="k">if</span> <span class="n">dunder</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
+</span><span id="Seats-52"><a href="#Seats-52"><span class="linenos">52</span></a>                <span class="n">init</span> <span class="o">=</span> <span class="n">dunders</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
+</span><span id="Seats-53"><a href="#Seats-53"><span class="linenos">53</span></a>                <span class="k">break</span>
+</span><span id="Seats-54"><a href="#Seats-54"><span class="linenos">54</span></a>        <span class="k">if</span> <span class="n">init</span><span class="p">:</span>
+</span><span id="Seats-55"><a href="#Seats-55"><span class="linenos">55</span></a>            <span class="n">dunders</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">init</span><span class="p">)</span>
+</span><span id="Seats-56"><a href="#Seats-56"><span class="linenos">56</span></a>        <span class="k">return</span> <span class="n">dunders</span>
+</span><span id="Seats-57"><a href="#Seats-57"><span class="linenos">57</span></a>
+</span><span id="Seats-58"><a href="#Seats-58"><span class="linenos">58</span></a>    <span class="k">def</span> <span class="nf">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">assigns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats-59"><a href="#Seats-59"><span class="linenos">59</span></a>        <span class="sd">&quot;&quot;&quot;Sort assignment statments.&quot;&quot;&quot;</span>
+</span><span id="Seats-60"><a href="#Seats-60"><span class="linenos">60</span></a>
+</span><span id="Seats-61"><a href="#Seats-61"><span class="linenos">61</span></a>        <span class="k">def</span> <span class="nf">get_name</span><span class="p">(</span><span class="n">node</span><span class="p">:</span> <span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Seats-62"><a href="#Seats-62"><span class="linenos">62</span></a>            <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">node</span><span class="p">)</span>
+</span><span id="Seats-63"><a href="#Seats-63"><span class="linenos">63</span></a>            <span class="k">if</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">:</span>
+</span><span id="Seats-64"><a href="#Seats-64"><span class="linenos">64</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">targets</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">id</span>
+</span><span id="Seats-65"><a href="#Seats-65"><span class="linenos">65</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Seats-66"><a href="#Seats-66"><span class="linenos">66</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">target</span><span class="o">.</span><span class="n">id</span>
+</span><span id="Seats-67"><a href="#Seats-67"><span class="linenos">67</span></a>
+</span><span id="Seats-68"><a href="#Seats-68"><span class="linenos">68</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">assigns</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="n">get_name</span><span class="p">)</span>
+</span><span id="Seats-69"><a href="#Seats-69"><span class="linenos">69</span></a>
+</span><span id="Seats-70"><a href="#Seats-70"><span class="linenos">70</span></a>    <span class="k">def</span> <span class="nf">sort</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats-71"><a href="#Seats-71"><span class="linenos">71</span></a>        <span class="sd">&quot;&quot;&quot;Sort and return members as a single list.&quot;&quot;&quot;</span>
+</span><span id="Seats-72"><a href="#Seats-72"><span class="linenos">72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dunders</span><span class="p">)</span>
+</span><span id="Seats-73"><a href="#Seats-73"><span class="linenos">73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">functions</span><span class="p">)</span>
+</span><span id="Seats-74"><a href="#Seats-74"><span class="linenos">74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">properties</span><span class="p">)</span>
+</span><span id="Seats-75"><a href="#Seats-75"><span class="linenos">75</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">assigns</span><span class="p">)</span>
+</span><span id="Seats-76"><a href="#Seats-76"><span class="linenos">76</span></a>        <span class="n">body</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="Seats-77"><a href="#Seats-77"><span class="linenos">77</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">before</span>
+</span><span id="Seats-78"><a href="#Seats-78"><span class="linenos">78</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span>
+</span><span id="Seats-79"><a href="#Seats-79"><span class="linenos">79</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span>
+</span><span id="Seats-80"><a href="#Seats-80"><span class="linenos">80</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">properties</span>
+</span><span id="Seats-81"><a href="#Seats-81"><span class="linenos">81</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">functions</span>
+</span><span id="Seats-82"><a href="#Seats-82"><span class="linenos">82</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">seats</span>
+</span><span id="Seats-83"><a href="#Seats-83"><span class="linenos">83</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">after</span>
+</span><span id="Seats-84"><a href="#Seats-84"><span class="linenos">84</span></a>        <span class="p">)</span>
+</span><span id="Seats-85"><a href="#Seats-85"><span class="linenos">85</span></a>        <span class="k">for</span> <span class="n">expression</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">expressions</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">comments</span><span class="p">:</span>
+</span><span id="Seats-86"><a href="#Seats-86"><span class="linenos">86</span></a>            <span class="n">body</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">expression</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">expression</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="Seats-87"><a href="#Seats-87"><span class="linenos">87</span></a>        <span class="k">return</span> <span class="n">body</span>
 </span></pre></div>
 
 
     
 
-                            <div id="Order.__init__" class="classattr">
-                                        <input id="Order.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="Seats.__init__" class="classattr">
+                                        <input id="Seats.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
-        <span class="name">Order</span><span class="signature pdoc-code condensed">()</span>
+        <span class="name">Seats</span><span class="signature pdoc-code condensed">()</span>
 
-                <label class="view-source-button" for="Order.__init__-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Seats.__init__-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Order.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Order.__init__-30"><a href="#Order.__init__-30"><span class="linenos">30</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Order.__init__-31"><a href="#Order.__init__-31"><span class="linenos">31</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">before</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order.__init__-32"><a href="#Order.__init__-32"><span class="linenos">32</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order.__init__-33"><a href="#Order.__init__-33"><span class="linenos">33</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order.__init__-34"><a href="#Order.__init__-34"><span class="linenos">34</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order.__init__-35"><a href="#Order.__init__-35"><span class="linenos">35</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order.__init__-36"><a href="#Order.__init__-36"><span class="linenos">36</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">after</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Order.__init__-37"><a href="#Order.__init__-37"><span class="linenos">37</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">seats</span> <span class="o">=</span> <span class="p">[]</span>
+    <a class="headerlink" href="#Seats.__init__"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Seats.__init__-30"><a href="#Seats.__init__-30"><span class="linenos">30</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Seats.__init__-31"><a href="#Seats.__init__-31"><span class="linenos">31</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">before</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-32"><a href="#Seats.__init__-32"><span class="linenos">32</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-33"><a href="#Seats.__init__-33"><span class="linenos">33</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-34"><a href="#Seats.__init__-34"><span class="linenos">34</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-35"><a href="#Seats.__init__-35"><span class="linenos">35</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-36"><a href="#Seats.__init__-36"><span class="linenos">36</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">after</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-37"><a href="#Seats.__init__-37"><span class="linenos">37</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">seats</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-38"><a href="#Seats.__init__-38"><span class="linenos">38</span></a>        <span class="c1"># These will be a list of tuples containing the node and the index it was found at</span>
+</span><span id="Seats.__init__-39"><a href="#Seats.__init__-39"><span class="linenos">39</span></a>        <span class="c1"># so they can be reinserted after sorting</span>
+</span><span id="Seats.__init__-40"><a href="#Seats.__init__-40"><span class="linenos">40</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">expressions</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Seats.__init__-41"><a href="#Seats.__init__-41"><span class="linenos">41</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">comments</span> <span class="o">=</span> <span class="p">[]</span>
 </span></pre></div>
 
 
     
 
                             </div>
-                            <div id="Order.sort_nodes_by_name" class="classattr">
-                                        <input id="Order.sort_nodes_by_name-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="Seats.sort_nodes_by_name" class="classattr">
+                                        <input id="Seats.sort_nodes_by_name-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">sort_nodes_by_name</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">nodes</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]</span>:</span></span>
 
-                <label class="view-source-button" for="Order.sort_nodes_by_name-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Seats.sort_nodes_by_name-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Order.sort_nodes_by_name"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Order.sort_nodes_by_name-39"><a href="#Order.sort_nodes_by_name-39"><span class="linenos">39</span></a>    <span class="k">def</span> <span class="nf">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">nodes</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order.sort_nodes_by_name-40"><a href="#Order.sort_nodes_by_name-40"><span class="linenos">40</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">nodes</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">node</span><span class="p">:</span> <span class="n">node</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+    <a class="headerlink" href="#Seats.sort_nodes_by_name"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Seats.sort_nodes_by_name-43"><a href="#Seats.sort_nodes_by_name-43"><span class="linenos">43</span></a>    <span class="k">def</span> <span class="nf">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">nodes</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats.sort_nodes_by_name-44"><a href="#Seats.sort_nodes_by_name-44"><span class="linenos">44</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">nodes</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">node</span><span class="p">:</span> <span class="n">node</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
-                            <div id="Order.sort_dunders" class="classattr">
-                                        <input id="Order.sort_dunders-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="Seats.sort_dunders" class="classattr">
+                                        <input id="Seats.sort_dunders-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">sort_dunders</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">dunders</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]</span>:</span></span>
 
-                <label class="view-source-button" for="Order.sort_dunders-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Seats.sort_dunders-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Order.sort_dunders"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Order.sort_dunders-42"><a href="#Order.sort_dunders-42"><span class="linenos">42</span></a>    <span class="k">def</span> <span class="nf">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dunders</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order.sort_dunders-43"><a href="#Order.sort_dunders-43"><span class="linenos">43</span></a>        <span class="sd">&quot;&quot;&quot;Sort `dunders` alphabetically, except `__init__` is placed at the front, if it exists.&quot;&quot;&quot;</span>
-</span><span id="Order.sort_dunders-44"><a href="#Order.sort_dunders-44"><span class="linenos">44</span></a>        <span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="n">dunders</span><span class="p">)</span>
-</span><span id="Order.sort_dunders-45"><a href="#Order.sort_dunders-45"><span class="linenos">45</span></a>        <span class="n">init</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="Order.sort_dunders-46"><a href="#Order.sort_dunders-46"><span class="linenos">46</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">dunder</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">dunders</span><span class="p">):</span>
-</span><span id="Order.sort_dunders-47"><a href="#Order.sort_dunders-47"><span class="linenos">47</span></a>            <span class="k">if</span> <span class="n">dunder</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
-</span><span id="Order.sort_dunders-48"><a href="#Order.sort_dunders-48"><span class="linenos">48</span></a>                <span class="n">init</span> <span class="o">=</span> <span class="n">dunders</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
-</span><span id="Order.sort_dunders-49"><a href="#Order.sort_dunders-49"><span class="linenos">49</span></a>                <span class="k">break</span>
-</span><span id="Order.sort_dunders-50"><a href="#Order.sort_dunders-50"><span class="linenos">50</span></a>        <span class="k">if</span> <span class="n">init</span><span class="p">:</span>
-</span><span id="Order.sort_dunders-51"><a href="#Order.sort_dunders-51"><span class="linenos">51</span></a>            <span class="n">dunders</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">init</span><span class="p">)</span>
-</span><span id="Order.sort_dunders-52"><a href="#Order.sort_dunders-52"><span class="linenos">52</span></a>        <span class="k">return</span> <span class="n">dunders</span>
+    <a class="headerlink" href="#Seats.sort_dunders"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Seats.sort_dunders-46"><a href="#Seats.sort_dunders-46"><span class="linenos">46</span></a>    <span class="k">def</span> <span class="nf">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dunders</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats.sort_dunders-47"><a href="#Seats.sort_dunders-47"><span class="linenos">47</span></a>        <span class="sd">&quot;&quot;&quot;Sort `dunders` alphabetically, except `__init__` is placed at the front, if it exists.&quot;&quot;&quot;</span>
+</span><span id="Seats.sort_dunders-48"><a href="#Seats.sort_dunders-48"><span class="linenos">48</span></a>        <span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="n">dunders</span><span class="p">)</span>
+</span><span id="Seats.sort_dunders-49"><a href="#Seats.sort_dunders-49"><span class="linenos">49</span></a>        <span class="n">init</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="Seats.sort_dunders-50"><a href="#Seats.sort_dunders-50"><span class="linenos">50</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">dunder</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">dunders</span><span class="p">):</span>
+</span><span id="Seats.sort_dunders-51"><a href="#Seats.sort_dunders-51"><span class="linenos">51</span></a>            <span class="k">if</span> <span class="n">dunder</span><span class="o">.</span><span class="n">name</span> <span class="o">==</span> <span class="s2">&quot;__init__&quot;</span><span class="p">:</span>
+</span><span id="Seats.sort_dunders-52"><a href="#Seats.sort_dunders-52"><span class="linenos">52</span></a>                <span class="n">init</span> <span class="o">=</span> <span class="n">dunders</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
+</span><span id="Seats.sort_dunders-53"><a href="#Seats.sort_dunders-53"><span class="linenos">53</span></a>                <span class="k">break</span>
+</span><span id="Seats.sort_dunders-54"><a href="#Seats.sort_dunders-54"><span class="linenos">54</span></a>        <span class="k">if</span> <span class="n">init</span><span class="p">:</span>
+</span><span id="Seats.sort_dunders-55"><a href="#Seats.sort_dunders-55"><span class="linenos">55</span></a>            <span class="n">dunders</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">init</span><span class="p">)</span>
+</span><span id="Seats.sort_dunders-56"><a href="#Seats.sort_dunders-56"><span class="linenos">56</span></a>        <span class="k">return</span> <span class="n">dunders</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Sort <code>dunders</code> alphabetically, except <code><a href="#Order.__init__">__init__</a></code> is placed at the front, if it exists.</p>
+            <div class="docstring"><p>Sort <code>dunders</code> alphabetically, except <code><a href="#Seats.__init__">__init__</a></code> is placed at the front, if it exists.</p>
 </div>
 
 
                             </div>
-                            <div id="Order.sort_assigns" class="classattr">
-                                        <input id="Order.sort_assigns-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="Seats.sort_assigns" class="classattr">
+                                        <input id="Seats.sort_assigns-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">sort_assigns</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">assigns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]</span>:</span></span>
 
-                <label class="view-source-button" for="Order.sort_assigns-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Seats.sort_assigns-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Order.sort_assigns"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Order.sort_assigns-54"><a href="#Order.sort_assigns-54"><span class="linenos">54</span></a>    <span class="k">def</span> <span class="nf">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">assigns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order.sort_assigns-55"><a href="#Order.sort_assigns-55"><span class="linenos">55</span></a>        <span class="sd">&quot;&quot;&quot;Sort assignment statments.&quot;&quot;&quot;</span>
-</span><span id="Order.sort_assigns-56"><a href="#Order.sort_assigns-56"><span class="linenos">56</span></a>
-</span><span id="Order.sort_assigns-57"><a href="#Order.sort_assigns-57"><span class="linenos">57</span></a>        <span class="k">def</span> <span class="nf">get_name</span><span class="p">(</span><span class="n">node</span><span class="p">:</span> <span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Order.sort_assigns-58"><a href="#Order.sort_assigns-58"><span class="linenos">58</span></a>            <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">node</span><span class="p">)</span>
-</span><span id="Order.sort_assigns-59"><a href="#Order.sort_assigns-59"><span class="linenos">59</span></a>            <span class="k">if</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">:</span>
-</span><span id="Order.sort_assigns-60"><a href="#Order.sort_assigns-60"><span class="linenos">60</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">targets</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">id</span>
-</span><span id="Order.sort_assigns-61"><a href="#Order.sort_assigns-61"><span class="linenos">61</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Order.sort_assigns-62"><a href="#Order.sort_assigns-62"><span class="linenos">62</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">target</span><span class="o">.</span><span class="n">id</span>
-</span><span id="Order.sort_assigns-63"><a href="#Order.sort_assigns-63"><span class="linenos">63</span></a>
-</span><span id="Order.sort_assigns-64"><a href="#Order.sort_assigns-64"><span class="linenos">64</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">assigns</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="n">get_name</span><span class="p">)</span>
+    <a class="headerlink" href="#Seats.sort_assigns"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Seats.sort_assigns-58"><a href="#Seats.sort_assigns-58"><span class="linenos">58</span></a>    <span class="k">def</span> <span class="nf">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">assigns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats.sort_assigns-59"><a href="#Seats.sort_assigns-59"><span class="linenos">59</span></a>        <span class="sd">&quot;&quot;&quot;Sort assignment statments.&quot;&quot;&quot;</span>
+</span><span id="Seats.sort_assigns-60"><a href="#Seats.sort_assigns-60"><span class="linenos">60</span></a>
+</span><span id="Seats.sort_assigns-61"><a href="#Seats.sort_assigns-61"><span class="linenos">61</span></a>        <span class="k">def</span> <span class="nf">get_name</span><span class="p">(</span><span class="n">node</span><span class="p">:</span> <span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Seats.sort_assigns-62"><a href="#Seats.sort_assigns-62"><span class="linenos">62</span></a>            <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">node</span><span class="p">)</span>
+</span><span id="Seats.sort_assigns-63"><a href="#Seats.sort_assigns-63"><span class="linenos">63</span></a>            <span class="k">if</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">:</span>
+</span><span id="Seats.sort_assigns-64"><a href="#Seats.sort_assigns-64"><span class="linenos">64</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">targets</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">id</span>
+</span><span id="Seats.sort_assigns-65"><a href="#Seats.sort_assigns-65"><span class="linenos">65</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Seats.sort_assigns-66"><a href="#Seats.sort_assigns-66"><span class="linenos">66</span></a>                <span class="k">return</span> <span class="n">node</span><span class="o">.</span><span class="n">target</span><span class="o">.</span><span class="n">id</span>
+</span><span id="Seats.sort_assigns-67"><a href="#Seats.sort_assigns-67"><span class="linenos">67</span></a>
+</span><span id="Seats.sort_assigns-68"><a href="#Seats.sort_assigns-68"><span class="linenos">68</span></a>        <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">assigns</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="n">get_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sort assignment statments.</p>
 </div>
 
 
                             </div>
-                            <div id="Order.sort" class="classattr">
-                                        <input id="Order.sort-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="Seats.sort" class="classattr">
+                                        <input id="Seats.sort-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">sort</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]</span>:</span></span>
 
-                <label class="view-source-button" for="Order.sort-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Seats.sort-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Order.sort"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Order.sort-66"><a href="#Order.sort-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">sort</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
-</span><span id="Order.sort-67"><a href="#Order.sort-67"><span class="linenos">67</span></a>        <span class="sd">&quot;&quot;&quot;Sort and return members as a single list.&quot;&quot;&quot;</span>
-</span><span id="Order.sort-68"><a href="#Order.sort-68"><span class="linenos">68</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dunders</span><span class="p">)</span>
-</span><span id="Order.sort-69"><a href="#Order.sort-69"><span class="linenos">69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">functions</span><span class="p">)</span>
-</span><span id="Order.sort-70"><a href="#Order.sort-70"><span class="linenos">70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">properties</span><span class="p">)</span>
-</span><span id="Order.sort-71"><a href="#Order.sort-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">assigns</span><span class="p">)</span>
-</span><span id="Order.sort-72"><a href="#Order.sort-72"><span class="linenos">72</span></a>        <span class="k">return</span> <span class="p">(</span>
-</span><span id="Order.sort-73"><a href="#Order.sort-73"><span class="linenos">73</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">before</span>
-</span><span id="Order.sort-74"><a href="#Order.sort-74"><span class="linenos">74</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span>
-</span><span id="Order.sort-75"><a href="#Order.sort-75"><span class="linenos">75</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span>
-</span><span id="Order.sort-76"><a href="#Order.sort-76"><span class="linenos">76</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">properties</span>
-</span><span id="Order.sort-77"><a href="#Order.sort-77"><span class="linenos">77</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">functions</span>
-</span><span id="Order.sort-78"><a href="#Order.sort-78"><span class="linenos">78</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">seats</span>
-</span><span id="Order.sort-79"><a href="#Order.sort-79"><span class="linenos">79</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">after</span>
-</span><span id="Order.sort-80"><a href="#Order.sort-80"><span class="linenos">80</span></a>        <span class="p">)</span>
+    <a class="headerlink" href="#Seats.sort"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Seats.sort-70"><a href="#Seats.sort-70"><span class="linenos">70</span></a>    <span class="k">def</span> <span class="nf">sort</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">stmt</span><span class="p">]:</span>
+</span><span id="Seats.sort-71"><a href="#Seats.sort-71"><span class="linenos">71</span></a>        <span class="sd">&quot;&quot;&quot;Sort and return members as a single list.&quot;&quot;&quot;</span>
+</span><span id="Seats.sort-72"><a href="#Seats.sort-72"><span class="linenos">72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_dunders</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dunders</span><span class="p">)</span>
+</span><span id="Seats.sort-73"><a href="#Seats.sort-73"><span class="linenos">73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">functions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">functions</span><span class="p">)</span>
+</span><span id="Seats.sort-74"><a href="#Seats.sort-74"><span class="linenos">74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">properties</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_nodes_by_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">properties</span><span class="p">)</span>
+</span><span id="Seats.sort-75"><a href="#Seats.sort-75"><span class="linenos">75</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_assigns</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">assigns</span><span class="p">)</span>
+</span><span id="Seats.sort-76"><a href="#Seats.sort-76"><span class="linenos">76</span></a>        <span class="n">body</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="Seats.sort-77"><a href="#Seats.sort-77"><span class="linenos">77</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">before</span>
+</span><span id="Seats.sort-78"><a href="#Seats.sort-78"><span class="linenos">78</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">assigns</span>
+</span><span id="Seats.sort-79"><a href="#Seats.sort-79"><span class="linenos">79</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">dunders</span>
+</span><span id="Seats.sort-80"><a href="#Seats.sort-80"><span class="linenos">80</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">properties</span>
+</span><span id="Seats.sort-81"><a href="#Seats.sort-81"><span class="linenos">81</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">functions</span>
+</span><span id="Seats.sort-82"><a href="#Seats.sort-82"><span class="linenos">82</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">seats</span>
+</span><span id="Seats.sort-83"><a href="#Seats.sort-83"><span class="linenos">83</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">after</span>
+</span><span id="Seats.sort-84"><a href="#Seats.sort-84"><span class="linenos">84</span></a>        <span class="p">)</span>
+</span><span id="Seats.sort-85"><a href="#Seats.sort-85"><span class="linenos">85</span></a>        <span class="k">for</span> <span class="n">expression</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">expressions</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">comments</span><span class="p">:</span>
+</span><span id="Seats.sort-86"><a href="#Seats.sort-86"><span class="linenos">86</span></a>            <span class="n">body</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">expression</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">expression</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="Seats.sort-87"><a href="#Seats.sort-87"><span class="linenos">87</span></a>        <span class="k">return</span> <span class="n">body</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sort and return members as a single list.</p>
 </div>
 
 
@@ -556,102 +589,101 @@
         <span class="def">def</span>
         <span class="name">seat</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">source</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="seat-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#seat"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="seat-83"><a href="#seat-83"><span class="linenos"> 83</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
-</span><span id="seat-84"><a href="#seat-84"><span class="linenos"> 84</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="seat-85"><a href="#seat-85"><span class="linenos"> 85</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="seat-86"><a href="#seat-86"><span class="linenos"> 86</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
-</span><span id="seat-87"><a href="#seat-87"><span class="linenos"> 87</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
-</span><span id="seat-88"><a href="#seat-88"><span class="linenos"> 88</span></a>
-</span><span id="seat-89"><a href="#seat-89"><span class="linenos"> 89</span></a><span class="sd">    The modified `source` will be returned.</span>
-</span><span id="seat-90"><a href="#seat-90"><span class="linenos"> 90</span></a>
-</span><span id="seat-91"><a href="#seat-91"><span class="linenos"> 91</span></a><span class="sd">    #### :params:</span>
-</span><span id="seat-92"><a href="#seat-92"><span class="linenos"> 92</span></a>
-</span><span id="seat-93"><a href="#seat-93"><span class="linenos"> 93</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
-</span><span id="seat-94"><a href="#seat-94"><span class="linenos"> 94</span></a>
-</span><span id="seat-95"><a href="#seat-95"><span class="linenos"> 95</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
-</span><span id="seat-96"><a href="#seat-96"><span class="linenos"> 96</span></a>
-</span><span id="seat-97"><a href="#seat-97"><span class="linenos"> 97</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
-</span><span id="seat-98"><a href="#seat-98"><span class="linenos"> 98</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="seat-90"><a href="#seat-90"><span class="linenos"> 90</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
+</span><span id="seat-91"><a href="#seat-91"><span class="linenos"> 91</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="seat-92"><a href="#seat-92"><span class="linenos"> 92</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="seat-93"><a href="#seat-93"><span class="linenos"> 93</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
+</span><span id="seat-94"><a href="#seat-94"><span class="linenos"> 94</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
+</span><span id="seat-95"><a href="#seat-95"><span class="linenos"> 95</span></a>
+</span><span id="seat-96"><a href="#seat-96"><span class="linenos"> 96</span></a><span class="sd">    The modified `source` will be returned.</span>
+</span><span id="seat-97"><a href="#seat-97"><span class="linenos"> 97</span></a>
+</span><span id="seat-98"><a href="#seat-98"><span class="linenos"> 98</span></a><span class="sd">    #### :params:</span>
 </span><span id="seat-99"><a href="#seat-99"><span class="linenos"> 99</span></a>
-</span><span id="seat-100"><a href="#seat-100"><span class="linenos">100</span></a><span class="sd">    Note: Comments that are in a class body, but not in a function will remain at the same line.</span>
+</span><span id="seat-100"><a href="#seat-100"><span class="linenos">100</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
 </span><span id="seat-101"><a href="#seat-101"><span class="linenos">101</span></a>
-</span><span id="seat-102"><a href="#seat-102"><span class="linenos">102</span></a><span class="sd">    i.e. if the source is:</span>
-</span><span id="seat-103"><a href="#seat-103"><span class="linenos">103</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
-</span><span id="seat-104"><a href="#seat-104"><span class="linenos">104</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
-</span><span id="seat-105"><a href="#seat-105"><span class="linenos">105</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="seat-106"><a href="#seat-106"><span class="linenos">106</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
-</span><span id="seat-107"><a href="#seat-107"><span class="linenos">107</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="seat-108"><a href="#seat-108"><span class="linenos">108</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
-</span><span id="seat-109"><a href="#seat-109"><span class="linenos">109</span></a>
-</span><span id="seat-110"><a href="#seat-110"><span class="linenos">110</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
-</span><span id="seat-111"><a href="#seat-111"><span class="linenos">111</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
-</span><span id="seat-112"><a href="#seat-112"><span class="linenos">112</span></a>
-</span><span id="seat-113"><a href="#seat-113"><span class="linenos">113</span></a><span class="sd">    #### :Sorting and Priority:</span>
+</span><span id="seat-102"><a href="#seat-102"><span class="linenos">102</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
+</span><span id="seat-103"><a href="#seat-103"><span class="linenos">103</span></a>
+</span><span id="seat-104"><a href="#seat-104"><span class="linenos">104</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
+</span><span id="seat-105"><a href="#seat-105"><span class="linenos">105</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
+</span><span id="seat-106"><a href="#seat-106"><span class="linenos">106</span></a>
+</span><span id="seat-107"><a href="#seat-107"><span class="linenos">107</span></a><span class="sd">    i.e. if the source is:</span>
+</span><span id="seat-108"><a href="#seat-108"><span class="linenos">108</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
+</span><span id="seat-109"><a href="#seat-109"><span class="linenos">109</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
+</span><span id="seat-110"><a href="#seat-110"><span class="linenos">110</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="seat-111"><a href="#seat-111"><span class="linenos">111</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
+</span><span id="seat-112"><a href="#seat-112"><span class="linenos">112</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="seat-113"><a href="#seat-113"><span class="linenos">113</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
 </span><span id="seat-114"><a href="#seat-114"><span class="linenos">114</span></a>
-</span><span id="seat-115"><a href="#seat-115"><span class="linenos">115</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
-</span><span id="seat-116"><a href="#seat-116"><span class="linenos">116</span></a><span class="sd">    * Dunder methods</span>
-</span><span id="seat-117"><a href="#seat-117"><span class="linenos">117</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
-</span><span id="seat-118"><a href="#seat-118"><span class="linenos">118</span></a><span class="sd">    * Class functions</span>
+</span><span id="seat-115"><a href="#seat-115"><span class="linenos">115</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
+</span><span id="seat-116"><a href="#seat-116"><span class="linenos">116</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
+</span><span id="seat-117"><a href="#seat-117"><span class="linenos">117</span></a>
+</span><span id="seat-118"><a href="#seat-118"><span class="linenos">118</span></a><span class="sd">    #### :Sorting and Priority:</span>
 </span><span id="seat-119"><a href="#seat-119"><span class="linenos">119</span></a>
-</span><span id="seat-120"><a href="#seat-120"><span class="linenos">120</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
-</span><span id="seat-121"><a href="#seat-121"><span class="linenos">121</span></a>
-</span><span id="seat-122"><a href="#seat-122"><span class="linenos">122</span></a><span class="sd">    The only exception is for dunder methods.</span>
-</span><span id="seat-123"><a href="#seat-123"><span class="linenos">123</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
-</span><span id="seat-124"><a href="#seat-124"><span class="linenos">124</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="seat-125"><a href="#seat-125"><span class="linenos">125</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="seat-126"><a href="#seat-126"><span class="linenos">126</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
-</span><span id="seat-127"><a href="#seat-127"><span class="linenos">127</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
-</span><span id="seat-128"><a href="#seat-128"><span class="linenos">128</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="seat-129"><a href="#seat-129"><span class="linenos">129</span></a>    <span class="n">comments</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="seat-130"><a href="#seat-130"><span class="linenos">130</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
-</span><span id="seat-131"><a href="#seat-131"><span class="linenos">131</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
-</span><span id="seat-132"><a href="#seat-132"><span class="linenos">132</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
-</span><span id="seat-133"><a href="#seat-133"><span class="linenos">133</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Order</span><span class="p">()</span>
-</span><span id="seat-134"><a href="#seat-134"><span class="linenos">134</span></a>                <span class="k">for</span> <span class="n">child</span> <span class="ow">in</span> <span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">:</span>
-</span><span id="seat-135"><a href="#seat-135"><span class="linenos">135</span></a>                    <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-136"><a href="#seat-136"><span class="linenos">136</span></a>                    <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
-</span><span id="seat-137"><a href="#seat-137"><span class="linenos">137</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-138"><a href="#seat-138"><span class="linenos">138</span></a>                    <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
-</span><span id="seat-139"><a href="#seat-139"><span class="linenos">139</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-140"><a href="#seat-140"><span class="linenos">140</span></a>                    <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
-</span><span id="seat-141"><a href="#seat-141"><span class="linenos">141</span></a>                        <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
-</span><span id="seat-142"><a href="#seat-142"><span class="linenos">142</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-143"><a href="#seat-143"><span class="linenos">143</span></a>                        <span class="k">else</span><span class="p">:</span>
-</span><span id="seat-144"><a href="#seat-144"><span class="linenos">144</span></a>                            <span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-145"><a href="#seat-145"><span class="linenos">145</span></a>                    <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
-</span><span id="seat-146"><a href="#seat-146"><span class="linenos">146</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-147"><a href="#seat-147"><span class="linenos">147</span></a>                    <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
-</span><span id="seat-148"><a href="#seat-148"><span class="linenos">148</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-149"><a href="#seat-149"><span class="linenos">149</span></a>                    <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="seat-150"><a href="#seat-150"><span class="linenos">150</span></a>                        <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="seat-151"><a href="#seat-151"><span class="linenos">151</span></a>                            <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
-</span><span id="seat-152"><a href="#seat-152"><span class="linenos">152</span></a>                            <span class="k">if</span> <span class="p">(</span>
-</span><span id="seat-153"><a href="#seat-153"><span class="linenos">153</span></a>                                <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
-</span><span id="seat-154"><a href="#seat-154"><span class="linenos">154</span></a>                                <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span> <span class="o">==</span> <span class="s2">&quot;property&quot;</span>
-</span><span id="seat-155"><a href="#seat-155"><span class="linenos">155</span></a>                            <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
-</span><span id="seat-156"><a href="#seat-156"><span class="linenos">156</span></a>                                <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
-</span><span id="seat-157"><a href="#seat-157"><span class="linenos">157</span></a>                                <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
-</span><span id="seat-158"><a href="#seat-158"><span class="linenos">158</span></a>                            <span class="p">):</span>
-</span><span id="seat-159"><a href="#seat-159"><span class="linenos">159</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-160"><a href="#seat-160"><span class="linenos">160</span></a>                                <span class="k">break</span>
-</span><span id="seat-161"><a href="#seat-161"><span class="linenos">161</span></a>                        <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
-</span><span id="seat-162"><a href="#seat-162"><span class="linenos">162</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-163"><a href="#seat-163"><span class="linenos">163</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="seat-164"><a href="#seat-164"><span class="linenos">164</span></a>                        <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-165"><a href="#seat-165"><span class="linenos">165</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
-</span><span id="seat-166"><a href="#seat-166"><span class="linenos">166</span></a>    <span class="c1"># Put comments back in</span>
-</span><span id="seat-167"><a href="#seat-167"><span class="linenos">167</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="seat-168"><a href="#seat-168"><span class="linenos">168</span></a>    <span class="k">for</span> <span class="n">comment</span> <span class="ow">in</span> <span class="n">comments</span><span class="p">:</span>
-</span><span id="seat-169"><a href="#seat-169"><span class="linenos">169</span></a>        <span class="n">source</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">comment</span><span class="o">.</span><span class="n">lineno</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="n">comment</span><span class="o">.</span><span class="n">col_offset</span><span class="si">}{</span><span class="n">comment</span><span class="o">.</span><span class="n">value</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="seat-170"><a href="#seat-170"><span class="linenos">170</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="seat-120"><a href="#seat-120"><span class="linenos">120</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
+</span><span id="seat-121"><a href="#seat-121"><span class="linenos">121</span></a><span class="sd">    * Dunder methods</span>
+</span><span id="seat-122"><a href="#seat-122"><span class="linenos">122</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
+</span><span id="seat-123"><a href="#seat-123"><span class="linenos">123</span></a><span class="sd">    * Class functions</span>
+</span><span id="seat-124"><a href="#seat-124"><span class="linenos">124</span></a>
+</span><span id="seat-125"><a href="#seat-125"><span class="linenos">125</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
+</span><span id="seat-126"><a href="#seat-126"><span class="linenos">126</span></a>
+</span><span id="seat-127"><a href="#seat-127"><span class="linenos">127</span></a><span class="sd">    The only exception is for dunder methods.</span>
+</span><span id="seat-128"><a href="#seat-128"><span class="linenos">128</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
+</span><span id="seat-129"><a href="#seat-129"><span class="linenos">129</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="seat-130"><a href="#seat-130"><span class="linenos">130</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="seat-131"><a href="#seat-131"><span class="linenos">131</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
+</span><span id="seat-132"><a href="#seat-132"><span class="linenos">132</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
+</span><span id="seat-133"><a href="#seat-133"><span class="linenos">133</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="seat-134"><a href="#seat-134"><span class="linenos">134</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
+</span><span id="seat-135"><a href="#seat-135"><span class="linenos">135</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="seat-136"><a href="#seat-136"><span class="linenos">136</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
+</span><span id="seat-137"><a href="#seat-137"><span class="linenos">137</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Seats</span><span class="p">()</span>
+</span><span id="seat-138"><a href="#seat-138"><span class="linenos">138</span></a>                <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">child</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="seat-139"><a href="#seat-139"><span class="linenos">139</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="seat-140"><a href="#seat-140"><span class="linenos">140</span></a>                        <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-141"><a href="#seat-141"><span class="linenos">141</span></a>                        <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
+</span><span id="seat-142"><a href="#seat-142"><span class="linenos">142</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-143"><a href="#seat-143"><span class="linenos">143</span></a>                        <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
+</span><span id="seat-144"><a href="#seat-144"><span class="linenos">144</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-145"><a href="#seat-145"><span class="linenos">145</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Expr</span><span class="p">:</span>
+</span><span id="seat-146"><a href="#seat-146"><span class="linenos">146</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">expressions</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="seat-147"><a href="#seat-147"><span class="linenos">147</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
+</span><span id="seat-148"><a href="#seat-148"><span class="linenos">148</span></a>                            <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
+</span><span id="seat-149"><a href="#seat-149"><span class="linenos">149</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-150"><a href="#seat-150"><span class="linenos">150</span></a>                            <span class="k">else</span><span class="p">:</span>
+</span><span id="seat-151"><a href="#seat-151"><span class="linenos">151</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="seat-152"><a href="#seat-152"><span class="linenos">152</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
+</span><span id="seat-153"><a href="#seat-153"><span class="linenos">153</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-154"><a href="#seat-154"><span class="linenos">154</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
+</span><span id="seat-155"><a href="#seat-155"><span class="linenos">155</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-156"><a href="#seat-156"><span class="linenos">156</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="seat-157"><a href="#seat-157"><span class="linenos">157</span></a>                            <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="seat-158"><a href="#seat-158"><span class="linenos">158</span></a>                                <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
+</span><span id="seat-159"><a href="#seat-159"><span class="linenos">159</span></a>                                <span class="k">if</span> <span class="p">(</span>
+</span><span id="seat-160"><a href="#seat-160"><span class="linenos">160</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
+</span><span id="seat-161"><a href="#seat-161"><span class="linenos">161</span></a>                                    <span class="ow">and</span> <span class="s2">&quot;property&quot;</span> <span class="ow">in</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span>
+</span><span id="seat-162"><a href="#seat-162"><span class="linenos">162</span></a>                                <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
+</span><span id="seat-163"><a href="#seat-163"><span class="linenos">163</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
+</span><span id="seat-164"><a href="#seat-164"><span class="linenos">164</span></a>                                    <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
+</span><span id="seat-165"><a href="#seat-165"><span class="linenos">165</span></a>                                <span class="p">):</span>
+</span><span id="seat-166"><a href="#seat-166"><span class="linenos">166</span></a>                                    <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-167"><a href="#seat-167"><span class="linenos">167</span></a>                                    <span class="k">break</span>
+</span><span id="seat-168"><a href="#seat-168"><span class="linenos">168</span></a>                            <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
+</span><span id="seat-169"><a href="#seat-169"><span class="linenos">169</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-170"><a href="#seat-170"><span class="linenos">170</span></a>                        <span class="k">else</span><span class="p">:</span>
+</span><span id="seat-171"><a href="#seat-171"><span class="linenos">171</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-172"><a href="#seat-172"><span class="linenos">172</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="seat-173"><a href="#seat-173"><span class="linenos">173</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">child</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">))</span>
+</span><span id="seat-174"><a href="#seat-174"><span class="linenos">174</span></a>                        <span class="k">raise</span> <span class="n">e</span>
+</span><span id="seat-175"><a href="#seat-175"><span class="linenos">175</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
+</span><span id="seat-176"><a href="#seat-176"><span class="linenos">176</span></a>    <span class="k">return</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sort the contents of classes in <code>source</code>, where <code>source</code> is parsable Python code.
 Anything not inside a class will be untouched.</p>
 
 <p>The modified <code>source</code> will be returned.</p>
@@ -662,16 +694,14 @@
 <li><p><code>start_line</code>: Only sort contents after this line.</p></li>
 <li><p><code>stop_line</code>: Only sort contents before this line.</p></li>
 </ul>
 
 <p>If you have class contents that are grouped a certain way and you want the groups individually sorted
 so that the grouping is maintained, you can use <code># Seat</code> to demarcate the groups.</p>
 
-<p>Note: Comments that are in a class body, but not in a function will remain at the same line.</p>
-
 <p>i.e. if the source is:</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="k">class</span> <span class="nc">MyClass</span><span class="p">():</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="p">{</span><span class="n">arbitrary</span> <span class="n">lines</span> <span class="n">of</span> <span class="n">code</span><span class="p">}</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># Seat</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="p">{</span><span class="n">more</span> <span class="n">arbitrary</span> <span class="n">code</span><span class="p">}</span>
@@ -707,45 +737,52 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-173"><a href="#get_args-173"><span class="linenos">173</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-174"><a href="#get_args-174"><span class="linenos">174</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-175"><a href="#get_args-175"><span class="linenos">175</span></a>
-</span><span id="get_args-176"><a href="#get_args-176"><span class="linenos">176</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
-</span><span id="get_args-177"><a href="#get_args-177"><span class="linenos">177</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-178"><a href="#get_args-178"><span class="linenos">178</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
-</span><span id="get_args-179"><a href="#get_args-179"><span class="linenos">179</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
-</span><span id="get_args-180"><a href="#get_args-180"><span class="linenos">180</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-181"><a href="#get_args-181"><span class="linenos">181</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-182"><a href="#get_args-182"><span class="linenos">182</span></a>    <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-179"><a href="#get_args-179"><span class="linenos">179</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-180"><a href="#get_args-180"><span class="linenos">180</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-181"><a href="#get_args-181"><span class="linenos">181</span></a>
+</span><span id="get_args-182"><a href="#get_args-182"><span class="linenos">182</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
 </span><span id="get_args-183"><a href="#get_args-183"><span class="linenos">183</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-184"><a href="#get_args-184"><span class="linenos">184</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
+</span><span id="get_args-184"><a href="#get_args-184"><span class="linenos">184</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
 </span><span id="get_args-185"><a href="#get_args-185"><span class="linenos">185</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
 </span><span id="get_args-186"><a href="#get_args-186"><span class="linenos">186</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-187"><a href="#get_args-187"><span class="linenos">187</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-187"><a href="#get_args-187"><span class="linenos">187</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="get_args-188"><a href="#get_args-188"><span class="linenos">188</span></a>    <span class="p">)</span>
 </span><span id="get_args-189"><a href="#get_args-189"><span class="linenos">189</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-190"><a href="#get_args-190"><span class="linenos">190</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
-</span><span id="get_args-191"><a href="#get_args-191"><span class="linenos">191</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
-</span><span id="get_args-192"><a href="#get_args-192"><span class="linenos">192</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-193"><a href="#get_args-193"><span class="linenos">193</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-190"><a href="#get_args-190"><span class="linenos">190</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
+</span><span id="get_args-191"><a href="#get_args-191"><span class="linenos">191</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
+</span><span id="get_args-192"><a href="#get_args-192"><span class="linenos">192</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-193"><a href="#get_args-193"><span class="linenos">193</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="get_args-194"><a href="#get_args-194"><span class="linenos">194</span></a>    <span class="p">)</span>
 </span><span id="get_args-195"><a href="#get_args-195"><span class="linenos">195</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-196"><a href="#get_args-196"><span class="linenos">196</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="get_args-197"><a href="#get_args-197"><span class="linenos">197</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
-</span><span id="get_args-198"><a href="#get_args-198"><span class="linenos">198</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-199"><a href="#get_args-199"><span class="linenos">199</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-196"><a href="#get_args-196"><span class="linenos">196</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
+</span><span id="get_args-197"><a href="#get_args-197"><span class="linenos">197</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
+</span><span id="get_args-198"><a href="#get_args-198"><span class="linenos">198</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-199"><a href="#get_args-199"><span class="linenos">199</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="get_args-200"><a href="#get_args-200"><span class="linenos">200</span></a>    <span class="p">)</span>
-</span><span id="get_args-201"><a href="#get_args-201"><span class="linenos">201</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-202"><a href="#get_args-202"><span class="linenos">202</span></a>
-</span><span id="get_args-203"><a href="#get_args-203"><span class="linenos">203</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="get_args-201"><a href="#get_args-201"><span class="linenos">201</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-202"><a href="#get_args-202"><span class="linenos">202</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="get_args-203"><a href="#get_args-203"><span class="linenos">203</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
+</span><span id="get_args-204"><a href="#get_args-204"><span class="linenos">204</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-205"><a href="#get_args-205"><span class="linenos">205</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-206"><a href="#get_args-206"><span class="linenos">206</span></a>    <span class="p">)</span>
+</span><span id="get_args-207"><a href="#get_args-207"><span class="linenos">207</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-208"><a href="#get_args-208"><span class="linenos">208</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="get_args-209"><a href="#get_args-209"><span class="linenos">209</span></a>        <span class="s2">&quot;--dump&quot;</span><span class="p">,</span>
+</span><span id="get_args-210"><a href="#get_args-210"><span class="linenos">210</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-211"><a href="#get_args-211"><span class="linenos">211</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Dump ast tree to file instead of doing anything else. </span>
+</span><span id="get_args-212"><a href="#get_args-212"><span class="linenos">212</span></a><span class="s2">        For debugging purposes.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-213"><a href="#get_args-213"><span class="linenos">213</span></a>    <span class="p">)</span>
+</span><span id="get_args-214"><a href="#get_args-214"><span class="linenos">214</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-215"><a href="#get_args-215"><span class="linenos">215</span></a>
+</span><span id="get_args-216"><a href="#get_args-216"><span class="linenos">216</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="main">
@@ -755,22 +792,28 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
-</span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
-</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
-</span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>    <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">dump</span><span class="p">:</span>
+</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span>
+</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_ast_dump.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>            <span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
+</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>        <span class="p">)</span>
+</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
+</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
+</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>            <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
+</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
 
   ⁰
 ____ seating [Unknown INPUT type]
 ***** API Documentation *****
     * get_seat_sections
-    * Order
-          o Order
+    * Seats
+          o Seats
           o sort_nodes_by_name
           o sort_dunders
           o sort_assigns
           o sort
     * seat
     * get_args
     * main
@@ -42,217 +42,236 @@
 _21                else:
 _22                    sections.append((previous_endline() + 1, i + 1))
 _23        sections.append((previous_endline() + 1, len(lines) + 1))
 _24        return sections
 _25    return [(1, len(source.splitlines()) + 1)]
 _26
 _27
-_28class Order:
+_28class Seats:
 _29    def __init__(self):
 _30        self.before = []
 _31        self.assigns = []
 _32        self.dunders = []
 _33        self.properties = []
 _34        self.functions = []
 _35        self.after = []
 _36        self.seats = []
-_37
-_38    def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]:
-_39        return sorted(nodes, key=lambda node: node.name)
-_40
-_41    def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]:
-_42        """Sort `dunders` alphabetically, except `__init__` is placed at the
+_37        # These will be a list of tuples containing the node and the index
+it was found at
+_38        # so they can be reinserted after sorting
+_39        self.expressions = []
+_40        self.comments = []
+_41
+_42    def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]:
+_43        return sorted(nodes, key=lambda node: node.name)
+_44
+_45    def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]:
+_46        """Sort `dunders` alphabetically, except `__init__` is placed at the
 front, if it exists."""
-_43        dunders = self.sort_nodes_by_name(dunders)
-_44        init = None
-_45        for i, dunder in enumerate(dunders):
-_46            if dunder.name == "__init__":
-_47                init = dunders.pop(i)
-_48                break
-_49        if init:
-_50            dunders.insert(0, init)
-_51        return dunders
-_52
-_53    def sort_assigns(self, assigns: list[ast.stmt]) -> list[ast.stmt]:
-_54        """Sort assignment statments."""
-_55
-_56        def get_name(node: ast.stmt) -> str:
-_57            type_ = type(node)
-_58            if type_ == ast.Assign:
-_59                return node.targets[0].id
-_60            else:
-_61                return node.target.id
-_62
-_63        return sorted(assigns, key=get_name)
-_64
-_65    def sort(self) -> list[ast.stmt]:
-_66        """Sort and return members as a single list."""
-_67        self.dunders = self.sort_dunders(self.dunders)
-_68        self.functions = self.sort_nodes_by_name(self.functions)
-_69        self.properties = self.sort_nodes_by_name(self.properties)
-_70        self.assigns = self.sort_assigns(self.assigns)
-_71        return (
-_72            self.before
-_73            + self.assigns
-_74            + self.dunders
-_75            + self.properties
-_76            + self.functions
-_77            + self.seats
-_78            + self.after
-_79        )
-_80
-_81
-_82def seat(
-_83    source: str, start_line: int | None = None, stop_line: int | None = None
-_84) -> str:
-_85    """Sort the contents of classes in `source`, where `source` is parsable
-Python code.
-_86    Anything not inside a class will be untouched.
+_47        dunders = self.sort_nodes_by_name(dunders)
+_48        init = None
+_49        for i, dunder in enumerate(dunders):
+_50            if dunder.name == "__init__":
+_51                init = dunders.pop(i)
+_52                break
+_53        if init:
+_54            dunders.insert(0, init)
+_55        return dunders
+_56
+_57    def sort_assigns(self, assigns: list[ast.stmt]) -> list[ast.stmt]:
+_58        """Sort assignment statments."""
+_59
+_60        def get_name(node: ast.stmt) -> str:
+_61            type_ = type(node)
+_62            if type_ == ast.Assign:
+_63                return node.targets[0].id
+_64            else:
+_65                return node.target.id
+_66
+_67        return sorted(assigns, key=get_name)
+_68
+_69    def sort(self) -> list[ast.stmt]:
+_70        """Sort and return members as a single list."""
+_71        self.dunders = self.sort_dunders(self.dunders)
+_72        self.functions = self.sort_nodes_by_name(self.functions)
+_73        self.properties = self.sort_nodes_by_name(self.properties)
+_74        self.assigns = self.sort_assigns(self.assigns)
+_75        body = (
+_76            self.before
+_77            + self.assigns
+_78            + self.dunders
+_79            + self.properties
+_80            + self.functions
+_81            + self.seats
+_82            + self.after
+_83        )
+_84        for expression in self.expressions + self.comments:
+_85            body.insert(expression[1], expression[0])
+_86        return body
 _87
-_88    The modified `source` will be returned.
-_89
-_90    #### :params:
-_91
-_92    * `start_line`: Only sort contents after this line.
-_93
-_94    * `stop_line`: Only sort contents before this line.
-_95
-_96    If you have class contents that are grouped a certain way and you want
-the groups individually sorted
-_97    so that the grouping is maintained, you can use `# Seat` to demarcate
-the groups.
+_88
+_89def seat(
+_90    source: str, start_line: int | None = None, stop_line: int | None = None
+_91) -> str:
+_92    """Sort the contents of classes in `source`, where `source` is parsable
+Python code.
+_93    Anything not inside a class will be untouched.
+_94
+_95    The modified `source` will be returned.
+_96
+_97    #### :params:
 _98
-_99    Note: Comments that are in a class body, but not in a function will
-remain at the same line.
+_99    * `start_line`: Only sort contents after this line.
 100
-101    i.e. if the source is:
-102    >>> class MyClass():
-103    >>>     {arbitrary lines of code}
-104    >>>     # Seat
-105    >>>     {more arbitrary code}
-106    >>>     # Seat
-107    >>>     {yet more code}
-108
-109    Then the three sets of code in brackets will be sorted independently
-from one another
-110    (assuming no values are given for `start_line` or `stop_line`).
-111
-112    #### :Sorting and Priority:
+101    * `stop_line`: Only sort contents before this line.
+102
+103    If you have class contents that are grouped a certain way and you want
+the groups individually sorted
+104    so that the grouping is maintained, you can use `# Seat` to demarcate
+the groups.
+105
+106    i.e. if the source is:
+107    >>> class MyClass():
+108    >>>     {arbitrary lines of code}
+109    >>>     # Seat
+110    >>>     {more arbitrary code}
+111    >>>     # Seat
+112    >>>     {yet more code}
 113
-114    * Class variables declared in class body outside of a function
-115    * Dunder methods
-116    * Functions decorated with `property` or corresponding `.setter` and
-`.deleter` methods
-117    * Class functions
+114    Then the three sets of code in brackets will be sorted independently
+from one another
+115    (assuming no values are given for `start_line` or `stop_line`).
+116
+117    #### :Sorting and Priority:
 118
-119    Each of these groups will be sorted alphabetically with respect to
+119    * Class variables declared in class body outside of a function
+120    * Dunder methods
+121    * Functions decorated with `property` or corresponding `.setter` and
+`.deleter` methods
+122    * Class functions
+123
+124    Each of these groups will be sorted alphabetically with respect to
 themselves.
-120
-121    The only exception is for dunder methods.
-122    They will be sorted alphabetically except that `__init__` will be first.
-123    """
-124    tree = ast.parse(source, type_comments=True)
-125    start_line = start_line or 0
-126    stop_line = stop_line or len(source.splitlines()) + 1
-127    sections = get_seat_sections(source)
-128    comments = []
-129    for section in sections:
-130        for i, stmt in enumerate(tree.body):
-131            if type(stmt) == ast.ClassDef:
-132                order = Order()
-133                for child in stmt.body:
-134                    type_ = type(child)
-135                    if child.lineno <= start_line or child.lineno < section
-[0]:
-136                        order.before.append(child)
-137                    elif stop_line < child.lineno or child.lineno > section
-[1]:
-138                        order.after.append(child)
-139                    elif type_ == ast.Comment:
-140                        if "# Seat" in child.value:
-141                            order.seats.append(child)
-142                        else:
-143                            comments.append(child)
-144                    elif type_ in [ast.Assign, ast.AugAssign,
+125
+126    The only exception is for dunder methods.
+127    They will be sorted alphabetically except that `__init__` will be first.
+128    """
+129    tree = ast.parse(source, type_comments=True)
+130    start_line = start_line or 0
+131    stop_line = stop_line or len(source.splitlines()) + 1
+132    sections = get_seat_sections(source)
+133    for section in sections:
+134        for i, stmt in enumerate(tree.body):
+135            if type(stmt) == ast.ClassDef:
+136                order = Seats()
+137                for j, child in enumerate(stmt.body):
+138                    try:
+139                        type_ = type(child)
+140                        if child.lineno <= start_line or child.lineno <
+section[0]:
+141                            order.before.append(child)
+142                        elif stop_line < child.lineno or child.lineno >
+section[1]:
+143                            order.after.append(child)
+144                        elif type_ == ast.Expr:
+145                            order.expressions.append((child, j))
+146                        elif type_ == ast.Comment:
+147                            if "# Seat" in child.value:
+148                                order.seats.append(child)
+149                            else:
+150                                order.comments.append((child, j))
+151                        elif type_ in [ast.Assign, ast.AugAssign,
 ast.AnnAssign]:
-145                        order.assigns.append(child)
-146                    elif child.name.startswith("__") and child.name.endswith
-("__"):
-147                        order.dunders.append(child)
-148                    elif child.decorator_list:
-149                        for decorator in child.decorator_list:
-150                            decorator_type = type(decorator)
-151                            if (
-152                                decorator_type == ast.Name
-153                                and decorator.id == "property"
-154                            ) or (
-155                                decorator_type == ast.Attribute
-156                                and decorator.attr in ["setter", "deleter"]
-157                            ):
-158                                order.properties.append(child)
-159                                break
-160                        if child not in order.properties:
-161                            order.functions.append(child)
-162                    else:
-163                        order.functions.append(child)
-164                tree.body[i].body = order.sort()
-165    # Put comments back in
-166    source = ast.unparse(tree).splitlines()
-167    for comment in comments:
-168        source.insert(comment.lineno - 1, f"{' '*comment.col_offset}
-{comment.value}")
-169    return "\n".join(source)
-170
-171
-172def get_args() -> argparse.Namespace:
-173    parser = argparse.ArgumentParser()
-174
-175    parser.add_argument("file", type=str, help=""" The file to format. """)
-176    parser.add_argument(
-177        "--start",
-178        type=int,
-179        default=None,
-180        help=""" Optional line number to start formatting at. """,
-181    )
+152                            order.assigns.append(child)
+153                        elif child.name.startswith("__") and
+child.name.endswith("__"):
+154                            order.dunders.append(child)
+155                        elif child.decorator_list:
+156                            for decorator in child.decorator_list:
+157                                decorator_type = type(decorator)
+158                                if (
+159                                    decorator_type == ast.Name
+160                                    and "property" in decorator.id
+161                                ) or (
+162                                    decorator_type == ast.Attribute
+163                                    and decorator.attr in ["setter",
+"deleter"]
+164                                ):
+165                                    order.properties.append(child)
+166                                    break
+167                            if child not in order.properties:
+168                                order.functions.append(child)
+169                        else:
+170                            order.functions.append(child)
+171                    except Exception as e:
+172                        print(ast.dump(child, indent=2))
+173                        raise e
+174                tree.body[i].body = order.sort()
+175    return ast.unparse(tree)
+176
+177
+178def get_args() -> argparse.Namespace:
+179    parser = argparse.ArgumentParser()
+180
+181    parser.add_argument("file", type=str, help=""" The file to format. """)
 182    parser.add_argument(
-183        "--stop",
+183        "--start",
 184        type=int,
 185        default=None,
-186        help=""" Optional line number to stop formatting at. """,
+186        help=""" Optional line number to start formatting at. """,
 187    )
 188    parser.add_argument(
-189        "-nb",
-190        "--noblack",
-191        action="store_true",
-192        help=""" Don't format file with Black after sorting. """,
+189        "--stop",
+190        type=int,
+191        default=None,
+192        help=""" Optional line number to stop formatting at. """,
 193    )
 194    parser.add_argument(
-195        "-o",
-196        "--output",
-197        default=None,
-198        help=""" Write changes to this file, otherwise changes are written
-back to the original file. """,
+195        "-nb",
+196        "--noblack",
+197        action="store_true",
+198        help=""" Don't format file with Black after sorting. """,
 199    )
-200    args = parser.parse_args()
-201
-202    return args
-203
-204
-205def main(args: argparse.Namespace | None = None):
-206    if not args:
-207        args = get_args()
-208    source = Pathier(args.file).read_text()
-209    source = seat(source, args.start, args.stop)
-210    if not args.noblack:
-211        source = black.format_str(source, mode=black.Mode())
-212    Pathier(args.output or args.file).write_text(source)
-213
+200    parser.add_argument(
+201        "-o",
+202        "--output",
+203        default=None,
+204        help=""" Write changes to this file, otherwise changes are written
+back to the original file. """,
+205    )
+206    parser.add_argument(
+207        "-d",
+208        "--dump",
+209        action="store_true",
+210        help=""" Dump ast tree to file instead of doing anything else.
+211        For debugging purposes.""",
+212    )
+213    args = parser.parse_args()
 214
-215if __name__ == "__main__":
-216    main(get_args())
+215    return args
+216
+217
+218def main(args: argparse.Namespace | None = None):
+219    if not args:
+220        args = get_args()
+221    source = Pathier(args.file).read_text()
+222    if args.dump:
+223        file = Pathier(args.file)
+224        file = file.with_name(f"{file.stem}_ast_dump.txt").write_text(
+225            ast.dump(ast.parse(source, type_comments=True), indent=2)
+226        )
+227    else:
+228        source = seat(source, args.start, args.stop)
+229        if not args.noblack:
+230            source = black.format_str(source, mode=black.Mode())
+231        Pathier(args.output or args.file).write_text(source)
+232
+233
+234if __name__ == "__main__":
+235    main(get_args())
   ⁰
 def get_seat_sections(source: str) -> list[tuple[int, int]]: View Source
 _9def get_seat_sections(source: str) -> list[tuple[int, int]]:
 10    """Return a list of line number pairs for content between `# Seat`
 comments in `source`.
 11
 12    If `source` has no `# Seat` comments, a list with one tuple will be
@@ -272,247 +291,259 @@
 25        return sections
 26    return [(1, len(source.splitlines()) + 1)]
 Return a list of line number pairs for content between # Seat comments in
 source.
 If source has no # Seat comments, a list with one tuple will be returned: [(1,
 number_of_lines_in_source)]
   ⁰
-class Order: View Source
-29class Order:
+class Seats: View Source
+29class Seats:
 30    def __init__(self):
 31        self.before = []
 32        self.assigns = []
 33        self.dunders = []
 34        self.properties = []
 35        self.functions = []
 36        self.after = []
 37        self.seats = []
-38
-39    def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]:
-40        return sorted(nodes, key=lambda node: node.name)
-41
-42    def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]:
-43        """Sort `dunders` alphabetically, except `__init__` is placed at the
+38        # These will be a list of tuples containing the node and the index it
+was found at
+39        # so they can be reinserted after sorting
+40        self.expressions = []
+41        self.comments = []
+42
+43    def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]:
+44        return sorted(nodes, key=lambda node: node.name)
+45
+46    def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]:
+47        """Sort `dunders` alphabetically, except `__init__` is placed at the
 front, if it exists."""
-44        dunders = self.sort_nodes_by_name(dunders)
-45        init = None
-46        for i, dunder in enumerate(dunders):
-47            if dunder.name == "__init__":
-48                init = dunders.pop(i)
-49                break
-50        if init:
-51            dunders.insert(0, init)
-52        return dunders
-53
-54    def sort_assigns(self, assigns: list[ast.stmt]) -> list[ast.stmt]:
-55        """Sort assignment statments."""
-56
-57        def get_name(node: ast.stmt) -> str:
-58            type_ = type(node)
-59            if type_ == ast.Assign:
-60                return node.targets[0].id
-61            else:
-62                return node.target.id
-63
-64        return sorted(assigns, key=get_name)
-65
-66    def sort(self) -> list[ast.stmt]:
-67        """Sort and return members as a single list."""
-68        self.dunders = self.sort_dunders(self.dunders)
-69        self.functions = self.sort_nodes_by_name(self.functions)
-70        self.properties = self.sort_nodes_by_name(self.properties)
-71        self.assigns = self.sort_assigns(self.assigns)
-72        return (
-73            self.before
-74            + self.assigns
-75            + self.dunders
-76            + self.properties
-77            + self.functions
-78            + self.seats
-79            + self.after
-80        )
+48        dunders = self.sort_nodes_by_name(dunders)
+49        init = None
+50        for i, dunder in enumerate(dunders):
+51            if dunder.name == "__init__":
+52                init = dunders.pop(i)
+53                break
+54        if init:
+55            dunders.insert(0, init)
+56        return dunders
+57
+58    def sort_assigns(self, assigns: list[ast.stmt]) -> list[ast.stmt]:
+59        """Sort assignment statments."""
+60
+61        def get_name(node: ast.stmt) -> str:
+62            type_ = type(node)
+63            if type_ == ast.Assign:
+64                return node.targets[0].id
+65            else:
+66                return node.target.id
+67
+68        return sorted(assigns, key=get_name)
+69
+70    def sort(self) -> list[ast.stmt]:
+71        """Sort and return members as a single list."""
+72        self.dunders = self.sort_dunders(self.dunders)
+73        self.functions = self.sort_nodes_by_name(self.functions)
+74        self.properties = self.sort_nodes_by_name(self.properties)
+75        self.assigns = self.sort_assigns(self.assigns)
+76        body = (
+77            self.before
+78            + self.assigns
+79            + self.dunders
+80            + self.properties
+81            + self.functions
+82            + self.seats
+83            + self.after
+84        )
+85        for expression in self.expressions + self.comments:
+86            body.insert(expression[1], expression[0])
+87        return body
 ⁰
-Order() View Source
+Seats() View Source
 30    def __init__(self):
 31        self.before = []
 32        self.assigns = []
 33        self.dunders = []
 34        self.properties = []
 35        self.functions = []
 36        self.after = []
 37        self.seats = []
+38        # These will be a list of tuples containing the node and the index it
+was found at
+39        # so they can be reinserted after sorting
+40        self.expressions = []
+41        self.comments = []
 ⁰
 def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]: View
 Source
-39    def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]:
-40        return sorted(nodes, key=lambda node: node.name)
+43    def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]:
+44        return sorted(nodes, key=lambda node: node.name)
 ⁰
 def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]: View Source
-42    def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]:
-43        """Sort `dunders` alphabetically, except `__init__` is placed at the
+46    def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]:
+47        """Sort `dunders` alphabetically, except `__init__` is placed at the
 front, if it exists."""
-44        dunders = self.sort_nodes_by_name(dunders)
-45        init = None
-46        for i, dunder in enumerate(dunders):
-47            if dunder.name == "__init__":
-48                init = dunders.pop(i)
-49                break
-50        if init:
-51            dunders.insert(0, init)
-52        return dunders
+48        dunders = self.sort_nodes_by_name(dunders)
+49        init = None
+50        for i, dunder in enumerate(dunders):
+51            if dunder.name == "__init__":
+52                init = dunders.pop(i)
+53                break
+54        if init:
+55            dunders.insert(0, init)
+56        return dunders
 Sort dunders alphabetically, except __init__ is placed at the front, if it
 exists.
 ⁰
 def sort_assigns(self, assigns: list[ast.stmt]) -> list[ast.stmt]: View Source
-54    def sort_assigns(self, assigns: list[ast.stmt]) -> list[ast.stmt]:
-55        """Sort assignment statments."""
-56
-57        def get_name(node: ast.stmt) -> str:
-58            type_ = type(node)
-59            if type_ == ast.Assign:
-60                return node.targets[0].id
-61            else:
-62                return node.target.id
-63
-64        return sorted(assigns, key=get_name)
+58    def sort_assigns(self, assigns: list[ast.stmt]) -> list[ast.stmt]:
+59        """Sort assignment statments."""
+60
+61        def get_name(node: ast.stmt) -> str:
+62            type_ = type(node)
+63            if type_ == ast.Assign:
+64                return node.targets[0].id
+65            else:
+66                return node.target.id
+67
+68        return sorted(assigns, key=get_name)
 Sort assignment statments.
 ⁰
 def sort(self) -> list[ast.stmt]: View Source
-66    def sort(self) -> list[ast.stmt]:
-67        """Sort and return members as a single list."""
-68        self.dunders = self.sort_dunders(self.dunders)
-69        self.functions = self.sort_nodes_by_name(self.functions)
-70        self.properties = self.sort_nodes_by_name(self.properties)
-71        self.assigns = self.sort_assigns(self.assigns)
-72        return (
-73            self.before
-74            + self.assigns
-75            + self.dunders
-76            + self.properties
-77            + self.functions
-78            + self.seats
-79            + self.after
-80        )
+70    def sort(self) -> list[ast.stmt]:
+71        """Sort and return members as a single list."""
+72        self.dunders = self.sort_dunders(self.dunders)
+73        self.functions = self.sort_nodes_by_name(self.functions)
+74        self.properties = self.sort_nodes_by_name(self.properties)
+75        self.assigns = self.sort_assigns(self.assigns)
+76        body = (
+77            self.before
+78            + self.assigns
+79            + self.dunders
+80            + self.properties
+81            + self.functions
+82            + self.seats
+83            + self.after
+84        )
+85        for expression in self.expressions + self.comments:
+86            body.insert(expression[1], expression[0])
+87        return body
 Sort and return members as a single list.
   ⁰
 def seat(
 source: str,
 start_line: int | None = None,
 stop_line: int | None = None) -> str: View Source
-_83def seat(
-_84    source: str, start_line: int | None = None, stop_line: int | None = None
-_85) -> str:
-_86    """Sort the contents of classes in `source`, where `source` is parsable
+_90def seat(
+_91    source: str, start_line: int | None = None, stop_line: int | None = None
+_92) -> str:
+_93    """Sort the contents of classes in `source`, where `source` is parsable
 Python code.
-_87    Anything not inside a class will be untouched.
-_88
-_89    The modified `source` will be returned.
-_90
-_91    #### :params:
-_92
-_93    * `start_line`: Only sort contents after this line.
-_94
-_95    * `stop_line`: Only sort contents before this line.
-_96
-_97    If you have class contents that are grouped a certain way and you want
-the groups individually sorted
-_98    so that the grouping is maintained, you can use `# Seat` to demarcate
-the groups.
+_94    Anything not inside a class will be untouched.
+_95
+_96    The modified `source` will be returned.
+_97
+_98    #### :params:
 _99
-100    Note: Comments that are in a class body, but not in a function will
-remain at the same line.
+100    * `start_line`: Only sort contents after this line.
 101
-102    i.e. if the source is:
-103    >>> class MyClass():
-104    >>>     {arbitrary lines of code}
-105    >>>     # Seat
-106    >>>     {more arbitrary code}
-107    >>>     # Seat
-108    >>>     {yet more code}
-109
-110    Then the three sets of code in brackets will be sorted independently
-from one another
-111    (assuming no values are given for `start_line` or `stop_line`).
-112
-113    #### :Sorting and Priority:
+102    * `stop_line`: Only sort contents before this line.
+103
+104    If you have class contents that are grouped a certain way and you want
+the groups individually sorted
+105    so that the grouping is maintained, you can use `# Seat` to demarcate
+the groups.
+106
+107    i.e. if the source is:
+108    >>> class MyClass():
+109    >>>     {arbitrary lines of code}
+110    >>>     # Seat
+111    >>>     {more arbitrary code}
+112    >>>     # Seat
+113    >>>     {yet more code}
 114
-115    * Class variables declared in class body outside of a function
-116    * Dunder methods
-117    * Functions decorated with `property` or corresponding `.setter` and
-`.deleter` methods
-118    * Class functions
+115    Then the three sets of code in brackets will be sorted independently
+from one another
+116    (assuming no values are given for `start_line` or `stop_line`).
+117
+118    #### :Sorting and Priority:
 119
-120    Each of these groups will be sorted alphabetically with respect to
+120    * Class variables declared in class body outside of a function
+121    * Dunder methods
+122    * Functions decorated with `property` or corresponding `.setter` and
+`.deleter` methods
+123    * Class functions
+124
+125    Each of these groups will be sorted alphabetically with respect to
 themselves.
-121
-122    The only exception is for dunder methods.
-123    They will be sorted alphabetically except that `__init__` will be first.
-124    """
-125    tree = ast.parse(source, type_comments=True)
-126    start_line = start_line or 0
-127    stop_line = stop_line or len(source.splitlines()) + 1
-128    sections = get_seat_sections(source)
-129    comments = []
-130    for section in sections:
-131        for i, stmt in enumerate(tree.body):
-132            if type(stmt) == ast.ClassDef:
-133                order = Order()
-134                for child in stmt.body:
-135                    type_ = type(child)
-136                    if child.lineno <= start_line or child.lineno < section
-[0]:
-137                        order.before.append(child)
-138                    elif stop_line < child.lineno or child.lineno > section
-[1]:
-139                        order.after.append(child)
-140                    elif type_ == ast.Comment:
-141                        if "# Seat" in child.value:
-142                            order.seats.append(child)
-143                        else:
-144                            comments.append(child)
-145                    elif type_ in [ast.Assign, ast.AugAssign,
+126
+127    The only exception is for dunder methods.
+128    They will be sorted alphabetically except that `__init__` will be first.
+129    """
+130    tree = ast.parse(source, type_comments=True)
+131    start_line = start_line or 0
+132    stop_line = stop_line or len(source.splitlines()) + 1
+133    sections = get_seat_sections(source)
+134    for section in sections:
+135        for i, stmt in enumerate(tree.body):
+136            if type(stmt) == ast.ClassDef:
+137                order = Seats()
+138                for j, child in enumerate(stmt.body):
+139                    try:
+140                        type_ = type(child)
+141                        if child.lineno <= start_line or child.lineno <
+section[0]:
+142                            order.before.append(child)
+143                        elif stop_line < child.lineno or child.lineno >
+section[1]:
+144                            order.after.append(child)
+145                        elif type_ == ast.Expr:
+146                            order.expressions.append((child, j))
+147                        elif type_ == ast.Comment:
+148                            if "# Seat" in child.value:
+149                                order.seats.append(child)
+150                            else:
+151                                order.comments.append((child, j))
+152                        elif type_ in [ast.Assign, ast.AugAssign,
 ast.AnnAssign]:
-146                        order.assigns.append(child)
-147                    elif child.name.startswith("__") and child.name.endswith
-("__"):
-148                        order.dunders.append(child)
-149                    elif child.decorator_list:
-150                        for decorator in child.decorator_list:
-151                            decorator_type = type(decorator)
-152                            if (
-153                                decorator_type == ast.Name
-154                                and decorator.id == "property"
-155                            ) or (
-156                                decorator_type == ast.Attribute
-157                                and decorator.attr in ["setter", "deleter"]
-158                            ):
-159                                order.properties.append(child)
-160                                break
-161                        if child not in order.properties:
-162                            order.functions.append(child)
-163                    else:
-164                        order.functions.append(child)
-165                tree.body[i].body = order.sort()
-166    # Put comments back in
-167    source = ast.unparse(tree).splitlines()
-168    for comment in comments:
-169        source.insert(comment.lineno - 1, f"{' '*comment.col_offset}
-{comment.value}")
-170    return "\n".join(source)
+153                            order.assigns.append(child)
+154                        elif child.name.startswith("__") and
+child.name.endswith("__"):
+155                            order.dunders.append(child)
+156                        elif child.decorator_list:
+157                            for decorator in child.decorator_list:
+158                                decorator_type = type(decorator)
+159                                if (
+160                                    decorator_type == ast.Name
+161                                    and "property" in decorator.id
+162                                ) or (
+163                                    decorator_type == ast.Attribute
+164                                    and decorator.attr in ["setter",
+"deleter"]
+165                                ):
+166                                    order.properties.append(child)
+167                                    break
+168                            if child not in order.properties:
+169                                order.functions.append(child)
+170                        else:
+171                            order.functions.append(child)
+172                    except Exception as e:
+173                        print(ast.dump(child, indent=2))
+174                        raise e
+175                tree.body[i].body = order.sort()
+176    return ast.unparse(tree)
 Sort the contents of classes in source, where source is parsable Python code.
 Anything not inside a class will be untouched.
 The modified source will be returned.
 *** :params: ***
     * start_line: Only sort contents after this line.
     * stop_line: Only sort contents before this line.
 If you have class contents that are grouped a certain way and you want the
 groups individually sorted so that the grouping is maintained, you can use #
 Seat to demarcate the groups.
-Note: Comments that are in a class body, but not in a function will remain at
-the same line.
 i.e. if the source is:
 >>> class MyClass():
 >>>     {arbitrary lines of code}
 >>>     # Seat
 >>>     {more arbitrary code}
 >>>     # Seat
 >>>     {yet more code}
@@ -525,50 +556,63 @@
       methods
     * Class functions
 Each of these groups will be sorted alphabetically with respect to themselves.
 The only exception is for dunder methods. They will be sorted alphabetically
 except that __init__ will be first.
   ⁰
 def get_args() -> argparse.Namespace: View Source
-173def get_args() -> argparse.Namespace:
-174    parser = argparse.ArgumentParser()
-175
-176    parser.add_argument("file", type=str, help=""" The file to format. """)
-177    parser.add_argument(
-178        "--start",
-179        type=int,
-180        default=None,
-181        help=""" Optional line number to start formatting at. """,
-182    )
+179def get_args() -> argparse.Namespace:
+180    parser = argparse.ArgumentParser()
+181
+182    parser.add_argument("file", type=str, help=""" The file to format. """)
 183    parser.add_argument(
-184        "--stop",
+184        "--start",
 185        type=int,
 186        default=None,
-187        help=""" Optional line number to stop formatting at. """,
+187        help=""" Optional line number to start formatting at. """,
 188    )
 189    parser.add_argument(
-190        "-nb",
-191        "--noblack",
-192        action="store_true",
-193        help=""" Don't format file with Black after sorting. """,
+190        "--stop",
+191        type=int,
+192        default=None,
+193        help=""" Optional line number to stop formatting at. """,
 194    )
 195    parser.add_argument(
-196        "-o",
-197        "--output",
-198        default=None,
-199        help=""" Write changes to this file, otherwise changes are written
-back to the original file. """,
+196        "-nb",
+197        "--noblack",
+198        action="store_true",
+199        help=""" Don't format file with Black after sorting. """,
 200    )
-201    args = parser.parse_args()
-202
-203    return args
+201    parser.add_argument(
+202        "-o",
+203        "--output",
+204        default=None,
+205        help=""" Write changes to this file, otherwise changes are written
+back to the original file. """,
+206    )
+207    parser.add_argument(
+208        "-d",
+209        "--dump",
+210        action="store_true",
+211        help=""" Dump ast tree to file instead of doing anything else.
+212        For debugging purposes.""",
+213    )
+214    args = parser.parse_args()
+215
+216    return args
   ⁰
 def main(args: argparse.Namespace | None = None): View Source
-206def main(args: argparse.Namespace | None = None):
-207    if not args:
-208        args = get_args()
-209    source = Pathier(args.file).read_text()
-210    source = seat(source, args.start, args.stop)
-211    if not args.noblack:
-212        source = black.format_str(source, mode=black.Mode())
-213    Pathier(args.output or args.file).write_text(source)
+219def main(args: argparse.Namespace | None = None):
+220    if not args:
+221        args = get_args()
+222    source = Pathier(args.file).read_text()
+223    if args.dump:
+224        file = Pathier(args.file)
+225        file = file.with_name(f"{file.stem}_ast_dump.txt").write_text(
+226            ast.dump(ast.parse(source, type_comments=True), indent=2)
+227        )
+228    else:
+229        source = seat(source, args.start, args.stop)
+230        if not args.noblack:
+231            source = black.format_str(source, mode=black.Mode())
+232        Pathier(args.output or args.file).write_text(source)
```

### Comparing `seating-0.0.0/src/seating/seating.py` & `seating-0.0.1/src/seating/seating.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,23 +21,27 @@
                 else:
                     sections.append((previous_endline() + 1, i + 1))
         sections.append((previous_endline() + 1, len(lines) + 1))
         return sections
     return [(1, len(source.splitlines()) + 1)]
 
 
-class Order:
+class Seats:
     def __init__(self):
         self.before = []
         self.assigns = []
         self.dunders = []
         self.properties = []
         self.functions = []
         self.after = []
         self.seats = []
+        # These will be a list of tuples containing the node and the index it was found at
+        # so they can be reinserted after sorting
+        self.expressions = []
+        self.comments = []
 
     def sort_nodes_by_name(self, nodes: list[ast.stmt]) -> list[ast.stmt]:
         return sorted(nodes, key=lambda node: node.name)
 
     def sort_dunders(self, dunders: list[ast.stmt]) -> list[ast.stmt]:
         """Sort `dunders` alphabetically, except `__init__` is placed at the front, if it exists."""
         dunders = self.sort_nodes_by_name(dunders)
@@ -64,23 +68,26 @@
 
     def sort(self) -> list[ast.stmt]:
         """Sort and return members as a single list."""
         self.dunders = self.sort_dunders(self.dunders)
         self.functions = self.sort_nodes_by_name(self.functions)
         self.properties = self.sort_nodes_by_name(self.properties)
         self.assigns = self.sort_assigns(self.assigns)
-        return (
+        body = (
             self.before
             + self.assigns
             + self.dunders
             + self.properties
             + self.functions
             + self.seats
             + self.after
         )
+        for expression in self.expressions + self.comments:
+            body.insert(expression[1], expression[0])
+        return body
 
 
 def seat(
     source: str, start_line: int | None = None, stop_line: int | None = None
 ) -> str:
     """Sort the contents of classes in `source`, where `source` is parsable Python code.
     Anything not inside a class will be untouched.
@@ -92,16 +99,14 @@
     * `start_line`: Only sort contents after this line.
 
     * `stop_line`: Only sort contents before this line.
 
     If you have class contents that are grouped a certain way and you want the groups individually sorted
     so that the grouping is maintained, you can use `# Seat` to demarcate the groups.
 
-    Note: Comments that are in a class body, but not in a function will remain at the same line.
-
     i.e. if the source is:
     >>> class MyClass():
     >>>     {arbitrary lines of code}
     >>>     # Seat
     >>>     {more arbitrary code}
     >>>     # Seat
     >>>     {yet more code}
@@ -121,56 +126,57 @@
     The only exception is for dunder methods.
     They will be sorted alphabetically except that `__init__` will be first.
     """
     tree = ast.parse(source, type_comments=True)
     start_line = start_line or 0
     stop_line = stop_line or len(source.splitlines()) + 1
     sections = get_seat_sections(source)
-    comments = []
     for section in sections:
         for i, stmt in enumerate(tree.body):
             if type(stmt) == ast.ClassDef:
-                order = Order()
-                for child in stmt.body:
-                    type_ = type(child)
-                    if child.lineno <= start_line or child.lineno < section[0]:
-                        order.before.append(child)
-                    elif stop_line < child.lineno or child.lineno > section[1]:
-                        order.after.append(child)
-                    elif type_ == ast.Comment:
-                        if "# Seat" in child.value:
-                            order.seats.append(child)
+                order = Seats()
+                for j, child in enumerate(stmt.body):
+                    try:
+                        type_ = type(child)
+                        if child.lineno <= start_line or child.lineno < section[0]:
+                            order.before.append(child)
+                        elif stop_line < child.lineno or child.lineno > section[1]:
+                            order.after.append(child)
+                        elif type_ == ast.Expr:
+                            order.expressions.append((child, j))
+                        elif type_ == ast.Comment:
+                            if "# Seat" in child.value:
+                                order.seats.append(child)
+                            else:
+                                order.comments.append((child, j))
+                        elif type_ in [ast.Assign, ast.AugAssign, ast.AnnAssign]:
+                            order.assigns.append(child)
+                        elif child.name.startswith("__") and child.name.endswith("__"):
+                            order.dunders.append(child)
+                        elif child.decorator_list:
+                            for decorator in child.decorator_list:
+                                decorator_type = type(decorator)
+                                if (
+                                    decorator_type == ast.Name
+                                    and "property" in decorator.id
+                                ) or (
+                                    decorator_type == ast.Attribute
+                                    and decorator.attr in ["setter", "deleter"]
+                                ):
+                                    order.properties.append(child)
+                                    break
+                            if child not in order.properties:
+                                order.functions.append(child)
                         else:
-                            comments.append(child)
-                    elif type_ in [ast.Assign, ast.AugAssign, ast.AnnAssign]:
-                        order.assigns.append(child)
-                    elif child.name.startswith("__") and child.name.endswith("__"):
-                        order.dunders.append(child)
-                    elif child.decorator_list:
-                        for decorator in child.decorator_list:
-                            decorator_type = type(decorator)
-                            if (
-                                decorator_type == ast.Name
-                                and decorator.id == "property"
-                            ) or (
-                                decorator_type == ast.Attribute
-                                and decorator.attr in ["setter", "deleter"]
-                            ):
-                                order.properties.append(child)
-                                break
-                        if child not in order.properties:
                             order.functions.append(child)
-                    else:
-                        order.functions.append(child)
+                    except Exception as e:
+                        print(ast.dump(child, indent=2))
+                        raise e
                 tree.body[i].body = order.sort()
-    # Put comments back in
-    source = ast.unparse(tree).splitlines()
-    for comment in comments:
-        source.insert(comment.lineno - 1, f"{' '*comment.col_offset}{comment.value}")
-    return "\n".join(source)
+    return ast.unparse(tree)
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument("file", type=str, help=""" The file to format. """)
     parser.add_argument(
@@ -193,24 +199,37 @@
     )
     parser.add_argument(
         "-o",
         "--output",
         default=None,
         help=""" Write changes to this file, otherwise changes are written back to the original file. """,
     )
+    parser.add_argument(
+        "-d",
+        "--dump",
+        action="store_true",
+        help=""" Dump ast tree to file instead of doing anything else. 
+        For debugging purposes.""",
+    )
     args = parser.parse_args()
 
     return args
 
 
 def main(args: argparse.Namespace | None = None):
     if not args:
         args = get_args()
     source = Pathier(args.file).read_text()
-    source = seat(source, args.start, args.stop)
-    if not args.noblack:
-        source = black.format_str(source, mode=black.Mode())
-    Pathier(args.output or args.file).write_text(source)
+    if args.dump:
+        file = Pathier(args.file)
+        file = file.with_name(f"{file.stem}_ast_dump.txt").write_text(
+            ast.dump(ast.parse(source, type_comments=True), indent=2)
+        )
+    else:
+        source = seat(source, args.start, args.stop)
+        if not args.noblack:
+            source = black.format_str(source, mode=black.Mode())
+        Pathier(args.output or args.file).write_text(source)
 
 
 if __name__ == "__main__":
     main(get_args())
```

### Comparing `seating-0.0.0/LICENSE.txt` & `seating-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seating-0.0.0/README.md` & `seating-0.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -37,35 +37,33 @@
     {more arbitrary code}
     # Seat
     {yet more code}
 </pre>
 
 then the three sets of code in brackets will be sorted independently from one another.
 
-Note: Comments that are in a class body, but not in a function will remain at the same line.<br>
-This can result in them being place in odd places after the file is sorted.
-
 ## Usage
 
 #### CLI
 
 <pre>
 >seat -h
-usage: seat [-h] [--start START] [--stop STOP] [-nb] [-o OUTPUT] file
+usage: seat [-h] [--start START] [--stop STOP] [-nb] [-o OUTPUT] [-d] file
 
 positional arguments:
   file                  The file to format.
 
 options:
   -h, --help            show this help message and exit
   --start START         Optional line number to start formatting at.
   --stop STOP           Optional line number to stop formatting at.
   -nb, --noblack        Don't format file with Black after sorting.
   -o OUTPUT, --output OUTPUT
                         Write changes to this file, otherwise changes are written back to the original file.
+  -d, --dump            Dump ast tree to file instead of doing anything else. For debugging purposes.
 </pre>
 
 #### Programmatically
 
 <pre>
 from seating import seat
 from pathier import Pathier
```

### Comparing `seating-0.0.0/pyproject.toml` & `seating-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 7365 6174 696e 6722 0d0a 6465 7363   "seating"..desc
 00000070: 7269 7074 696f 6e20 3d20 2253 6f72 7420  ription = "Sort 
 00000080: 7468 6520 6f72 6465 7220 6f66 2063 6c61  the order of cla
 00000090: 7373 2066 756e 6374 696f 6e73 2061 6e64  ss functions and
 000000a0: 2070 726f 7065 7274 6965 7322 0d0a 7665   properties"..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e30 2e30 220d  rsion = "0.0.0".
+000000b0: 7273 696f 6e20 3d20 2230 2e30 2e31 220d  rsion = "0.0.1".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6173  endencies = ["as
 000000f0: 745f 636f 6d6d 656e 7473 222c 2022 626c  t_comments", "bl
 00000100: 6163 6b22 2c20 2270 6174 6869 6572 222c  ack", "pathier",
 00000110: 2022 7079 7465 7374 225d 0d0a 7265 6164   "pytest"]..read
 00000120: 6d65 203d 2022 5245 4144 4d45 2e6d 6422  me = "README.md"
```

### Comparing `seating-0.0.0/PKG-INFO` & `seating-0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seating
-Version: 0.0.0
+Version: 0.0.1
 Summary: Sort the order of class functions and properties
 Project-URL: Homepage, https://github.com/matt-manes/seating
 Project-URL: Documentation, https://github.com/matt-manes/seating/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/seating/tree/main/src/seating
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: alphabetical,order,sort,style
@@ -57,35 +57,33 @@
     {more arbitrary code}
     # Seat
     {yet more code}
 </pre>
 
 then the three sets of code in brackets will be sorted independently from one another.
 
-Note: Comments that are in a class body, but not in a function will remain at the same line.<br>
-This can result in them being place in odd places after the file is sorted.
-
 ## Usage
 
 #### CLI
 
 <pre>
 >seat -h
-usage: seat [-h] [--start START] [--stop STOP] [-nb] [-o OUTPUT] file
+usage: seat [-h] [--start START] [--stop STOP] [-nb] [-o OUTPUT] [-d] file
 
 positional arguments:
   file                  The file to format.
 
 options:
   -h, --help            show this help message and exit
   --start START         Optional line number to start formatting at.
   --stop STOP           Optional line number to stop formatting at.
   -nb, --noblack        Don't format file with Black after sorting.
   -o OUTPUT, --output OUTPUT
                         Write changes to this file, otherwise changes are written back to the original file.
+  -d, --dump            Dump ast tree to file instead of doing anything else. For debugging purposes.
 </pre>
 
 #### Programmatically
 
 <pre>
 from seating import seat
 from pathier import Pathier
```

