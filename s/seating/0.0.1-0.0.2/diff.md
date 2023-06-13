# Comparing `tmp/seating-0.0.1.tar.gz` & `tmp/seating-0.0.2.tar.gz`

## Comparing `seating-0.0.1.tar` & `seating-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 seating-0.0.1/docs/index.html
--rw-r--r--   0        0        0    28083 2020-02-02 00:00:00.000000 seating-0.0.1/docs/search.js
--rw-r--r--   0        0        0    34048 2020-02-02 00:00:00.000000 seating-0.0.1/docs/seating.html
--rw-r--r--   0        0        0   171907 2020-02-02 00:00:00.000000 seating-0.0.1/docs/seating/seating.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 seating-0.0.1/src/seating/__init__.py
--rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 seating-0.0.1/src/seating/seating.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 seating-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 seating-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 seating-0.0.1/README.md
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 seating-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 seating-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 seating-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 seating-0.0.2/docs/index.html
+-rw-r--r--   0        0        0    29199 2020-02-02 00:00:00.000000 seating-0.0.2/docs/search.js
+-rw-r--r--   0        0        0    34048 2020-02-02 00:00:00.000000 seating-0.0.2/docs/seating.html
+-rw-r--r--   0        0        0   184660 2020-02-02 00:00:00.000000 seating-0.0.2/docs/seating/seating.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 seating-0.0.2/src/seating/__init__.py
+-rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 seating-0.0.2/src/seating/seating.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 seating-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 seating-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 seating-0.0.2/README.md
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 seating-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 seating-0.0.2/PKG-INFO
```

### Comparing `seating-0.0.1/docs/search.js` & `seating-0.0.2/docs/search.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -742,14 +742,22 @@
         "modulename": "seating.seating",
         "qualname": "Seats.sort",
         "kind": "function",
         "doc": "<p>Sort and return members as a single list.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">ast</span><span class=\"o\">.</span><span class=\"n\">stmt</span><span class=\"p\">]</span>:</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "seating.seating.fix_type_ignore",
+        "modulename": "seating.seating",
+        "qualname": "fix_type_ignore",
+        "kind": "function",
+        "doc": "<p>Fix misplacement of <code># type: ignore</code> comments in sorted <code>source</code>.</p>\n\n<p>Corrects when</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">var</span> <span class=\"o\">=</span> <span class=\"mi\">6</span> <span class=\"c1\"># type: ignore</span>\n</code></pre>\n</div>\n\n<p>gets turned into</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"c1\"># type: ignore</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">var</span> <span class=\"o\">=</span> <span class=\"mi\">6</span>\n</code></pre>\n</div>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">source</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "seating.seating.seat",
         "modulename": "seating.seating",
         "qualname": "seat",
         "kind": "function",
         "doc": "<p>Sort the contents of classes in <code>source</code>, where <code>source</code> is parsable Python code.\nAnything not inside a class will be untouched.</p>\n\n<p>The modified <code>source</code> will be returned.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<ul>\n<li><p><code>start_line</code>: Only sort contents after this line.</p></li>\n<li><p><code>stop_line</code>: Only sort contents before this line.</p></li>\n</ul>\n\n<p>If you have class contents that are grouped a certain way and you want the groups individually sorted\nso that the grouping is maintained, you can use <code># Seat</code> to demarcate the groups.</p>\n\n<p>i.e. if the source is:</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">class</span> <span class=\"nc\">MyClass</span><span class=\"p\">():</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">arbitrary</span> <span class=\"n\">lines</span> <span class=\"n\">of</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"c1\"># Seat</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">more</span> <span class=\"n\">arbitrary</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"c1\"># Seat</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"p\">{</span><span class=\"n\">yet</span> <span class=\"n\">more</span> <span class=\"n\">code</span><span class=\"p\">}</span>\n</code></pre>\n</div>\n\n<p>Then the three sets of code in brackets will be sorted independently from one another\n(assuming no values are given for <code>start_line</code> or <code>stop_line</code>).</p>\n\n<h4 id=\"sorting-and-priority\">:Sorting and Priority:</h4>\n\n<ul>\n<li>Class variables declared in class body outside of a function</li>\n<li>Dunder methods</li>\n<li>Functions decorated with <code>property</code> or corresponding <code>.setter</code> and <code>.deleter</code> methods</li>\n<li>Class functions</li>\n</ul>\n\n<p>Each of these groups will be sorted alphabetically with respect to themselves.</p>\n\n<p>The only exception is for dunder methods.\nThey will be sorted alphabetically except that <code>__init__</code> will be first.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">source</span><span class=\"p\">:</span> <span class=\"nb\">str</span>,</span><span class=\"param\">\t<span class=\"n\">start_line</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">stop_line</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
```

### Comparing `seating-0.0.1/docs/seating.html` & `seating-0.0.2/docs/seating.html`

 * *Files identical despite different names*

### Comparing `seating-0.0.1/docs/seating/seating.html` & `seating-0.0.2/docs/seating/seating.html`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,17 @@
                         <li>
                                 <a class="function" href="#Seats.sort">sort</a>
                         </li>
                 </ul>
 
             </li>
             <li>
+                    <a class="function" href="#fix_type_ignore">fix_type_ignore</a>
+            </li>
+            <li>
                     <a class="function" href="#seat">seat</a>
             </li>
             <li>
                     <a class="function" href="#get_args">get_args</a>
             </li>
             <li>
                     <a class="function" href="#main">main</a>
@@ -168,161 +171,182 @@
 </span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">after</span>
 </span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="p">)</span>
 </span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="k">for</span> <span class="n">expression</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">expressions</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">comments</span><span class="p">:</span>
 </span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>            <span class="n">body</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">expression</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">expression</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
 </span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="k">return</span> <span class="n">body</span>
 </span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
 </span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="k">def</span> <span class="nf">fix_type_ignore</span><span class="p">(</span><span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="sd">&quot;&quot;&quot;Fix misplacement of `# type: ignore` comments in sorted `source`.</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">    Corrects when</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">    &gt;&gt;&gt; var = 6 # type: ignore</span>
 </span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">    The modified `source` will be returned.</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">    gets turned into</span>
 </span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">    #### :params:</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">    i.e. if the source is:</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">    &gt;&gt;&gt; # type: ignore</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">    &gt;&gt;&gt; var = 6&quot;&quot;&quot;</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="n">lines</span> <span class="o">=</span> <span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="n">clean</span> <span class="o">=</span> <span class="k">lambda</span> <span class="n">s</span><span class="p">:</span> <span class="n">s</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">line</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">lines</span><span class="p">):</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="k">if</span> <span class="n">clean</span><span class="p">(</span><span class="n">line</span><span class="p">)</span> <span class="o">==</span> <span class="s2">&quot;#type:ignore&quot;</span> <span class="ow">and</span> <span class="mi">0</span> <span class="o">&lt;</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="nb">len</span><span class="p">(</span><span class="n">lines</span><span class="p">):</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>            <span class="n">lines</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>            <span class="k">if</span> <span class="s2">&quot;#type:ignore&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">clean</span><span class="p">(</span><span class="n">lines</span><span class="p">[</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]):</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                <span class="n">lines</span><span class="p">[</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="n">lines</span><span class="p">[</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;# type: ignore</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="k">return</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">lines</span><span class="p">)</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">    The modified `source` will be returned.</span>
 </span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">    #### :Sorting and Priority:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    * Dunder methods</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">    * Class functions</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
 </span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">    The only exception is for dunder methods.</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Seats</span><span class="p">()</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>                <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">child</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>                        <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                        <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>                        <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Expr</span><span class="p">:</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">expressions</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>                            <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>                            <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>                                <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>                                <span class="k">if</span> <span class="p">(</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>                                    <span class="ow">and</span> <span class="s2">&quot;property&quot;</span> <span class="ow">in</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                                <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                                    <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>                                <span class="p">):</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>                                    <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>                                    <span class="k">break</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>                            <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>                        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">child</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">))</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>                        <span class="k">raise</span> <span class="n">e</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="k">return</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="p">)</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="p">)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="p">)</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="p">)</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="s2">&quot;--dump&quot;</span><span class="p">,</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Dump ast tree to file instead of doing anything else. </span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="s2">        For debugging purposes.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="p">)</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">dump</span><span class="p">:</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_ast_dump.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>            <span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="p">)</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">    i.e. if the source is:</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">    #### :Sorting and Priority:</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">    * Dunder methods</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a><span class="sd">    * Class functions</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">    The only exception is for dunder methods.</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Seats</span><span class="p">()</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>                <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">child</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                        <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>                        <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                        <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Expr</span><span class="p">:</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">expressions</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>                            <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>                            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                            <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>                                <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>                                <span class="k">if</span> <span class="p">(</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>                                    <span class="ow">and</span> <span class="s2">&quot;property&quot;</span> <span class="ow">in</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>                                <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>                                    <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>                                <span class="p">):</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>                                    <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>                                    <span class="k">break</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>                            <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>                        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">child</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">))</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>                        <span class="k">raise</span> <span class="n">e</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="k">return</span> <span class="n">fix_type_ignore</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="p">)</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="p">)</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="p">)</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>    <span class="p">)</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="s2">&quot;--dump&quot;</span><span class="p">,</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Dump ast tree to file instead of doing anything else. </span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="s2">        For debugging purposes.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>    <span class="p">)</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">dump</span><span class="p">:</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_ast_dump.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>            <span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="p">)</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>            <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_seat_sections">
                             <input id="get_seat_sections-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -578,112 +602,165 @@
 
             <div class="docstring"><p>Sort and return members as a single list.</p>
 </div>
 
 
                             </div>
                 </section>
+                <section id="fix_type_ignore">
+                            <input id="fix_type_ignore-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">fix_type_ignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">source</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
+
+                <label class="view-source-button" for="fix_type_ignore-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#fix_type_ignore"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="fix_type_ignore-90"><a href="#fix_type_ignore-90"><span class="linenos"> 90</span></a><span class="k">def</span> <span class="nf">fix_type_ignore</span><span class="p">(</span><span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="fix_type_ignore-91"><a href="#fix_type_ignore-91"><span class="linenos"> 91</span></a>    <span class="sd">&quot;&quot;&quot;Fix misplacement of `# type: ignore` comments in sorted `source`.</span>
+</span><span id="fix_type_ignore-92"><a href="#fix_type_ignore-92"><span class="linenos"> 92</span></a>
+</span><span id="fix_type_ignore-93"><a href="#fix_type_ignore-93"><span class="linenos"> 93</span></a><span class="sd">    Corrects when</span>
+</span><span id="fix_type_ignore-94"><a href="#fix_type_ignore-94"><span class="linenos"> 94</span></a><span class="sd">    &gt;&gt;&gt; var = 6 # type: ignore</span>
+</span><span id="fix_type_ignore-95"><a href="#fix_type_ignore-95"><span class="linenos"> 95</span></a>
+</span><span id="fix_type_ignore-96"><a href="#fix_type_ignore-96"><span class="linenos"> 96</span></a><span class="sd">    gets turned into</span>
+</span><span id="fix_type_ignore-97"><a href="#fix_type_ignore-97"><span class="linenos"> 97</span></a>
+</span><span id="fix_type_ignore-98"><a href="#fix_type_ignore-98"><span class="linenos"> 98</span></a><span class="sd">    &gt;&gt;&gt; # type: ignore</span>
+</span><span id="fix_type_ignore-99"><a href="#fix_type_ignore-99"><span class="linenos"> 99</span></a><span class="sd">    &gt;&gt;&gt; var = 6&quot;&quot;&quot;</span>
+</span><span id="fix_type_ignore-100"><a href="#fix_type_ignore-100"><span class="linenos">100</span></a>    <span class="n">lines</span> <span class="o">=</span> <span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="fix_type_ignore-101"><a href="#fix_type_ignore-101"><span class="linenos">101</span></a>    <span class="n">clean</span> <span class="o">=</span> <span class="k">lambda</span> <span class="n">s</span><span class="p">:</span> <span class="n">s</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="fix_type_ignore-102"><a href="#fix_type_ignore-102"><span class="linenos">102</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">line</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">lines</span><span class="p">):</span>
+</span><span id="fix_type_ignore-103"><a href="#fix_type_ignore-103"><span class="linenos">103</span></a>        <span class="k">if</span> <span class="n">clean</span><span class="p">(</span><span class="n">line</span><span class="p">)</span> <span class="o">==</span> <span class="s2">&quot;#type:ignore&quot;</span> <span class="ow">and</span> <span class="mi">0</span> <span class="o">&lt;</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="nb">len</span><span class="p">(</span><span class="n">lines</span><span class="p">):</span>
+</span><span id="fix_type_ignore-104"><a href="#fix_type_ignore-104"><span class="linenos">104</span></a>            <span class="n">lines</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="fix_type_ignore-105"><a href="#fix_type_ignore-105"><span class="linenos">105</span></a>            <span class="k">if</span> <span class="s2">&quot;#type:ignore&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">clean</span><span class="p">(</span><span class="n">lines</span><span class="p">[</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]):</span>
+</span><span id="fix_type_ignore-106"><a href="#fix_type_ignore-106"><span class="linenos">106</span></a>                <span class="n">lines</span><span class="p">[</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="n">lines</span><span class="p">[</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;# type: ignore</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="fix_type_ignore-107"><a href="#fix_type_ignore-107"><span class="linenos">107</span></a>    <span class="k">return</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">lines</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Fix misplacement of <code># type: ignore</code> comments in sorted <code>source</code>.</p>
+
+<p>Corrects when</p>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">var</span> <span class="o">=</span> <span class="mi">6</span> <span class="c1"># type: ignore</span>
+</code></pre>
+</div>
+
+<p>gets turned into</p>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="c1"># type: ignore</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">var</span> <span class="o">=</span> <span class="mi">6</span>
+</code></pre>
+</div>
+</div>
+
+
+                </section>
                 <section id="seat">
                             <input id="seat-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">seat</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">source</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="seat-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#seat"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="seat-90"><a href="#seat-90"><span class="linenos"> 90</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
-</span><span id="seat-91"><a href="#seat-91"><span class="linenos"> 91</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="seat-92"><a href="#seat-92"><span class="linenos"> 92</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="seat-93"><a href="#seat-93"><span class="linenos"> 93</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
-</span><span id="seat-94"><a href="#seat-94"><span class="linenos"> 94</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
-</span><span id="seat-95"><a href="#seat-95"><span class="linenos"> 95</span></a>
-</span><span id="seat-96"><a href="#seat-96"><span class="linenos"> 96</span></a><span class="sd">    The modified `source` will be returned.</span>
-</span><span id="seat-97"><a href="#seat-97"><span class="linenos"> 97</span></a>
-</span><span id="seat-98"><a href="#seat-98"><span class="linenos"> 98</span></a><span class="sd">    #### :params:</span>
-</span><span id="seat-99"><a href="#seat-99"><span class="linenos"> 99</span></a>
-</span><span id="seat-100"><a href="#seat-100"><span class="linenos">100</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
-</span><span id="seat-101"><a href="#seat-101"><span class="linenos">101</span></a>
-</span><span id="seat-102"><a href="#seat-102"><span class="linenos">102</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
-</span><span id="seat-103"><a href="#seat-103"><span class="linenos">103</span></a>
-</span><span id="seat-104"><a href="#seat-104"><span class="linenos">104</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
-</span><span id="seat-105"><a href="#seat-105"><span class="linenos">105</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
-</span><span id="seat-106"><a href="#seat-106"><span class="linenos">106</span></a>
-</span><span id="seat-107"><a href="#seat-107"><span class="linenos">107</span></a><span class="sd">    i.e. if the source is:</span>
-</span><span id="seat-108"><a href="#seat-108"><span class="linenos">108</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
-</span><span id="seat-109"><a href="#seat-109"><span class="linenos">109</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
-</span><span id="seat-110"><a href="#seat-110"><span class="linenos">110</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="seat-111"><a href="#seat-111"><span class="linenos">111</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
-</span><span id="seat-112"><a href="#seat-112"><span class="linenos">112</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
-</span><span id="seat-113"><a href="#seat-113"><span class="linenos">113</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
-</span><span id="seat-114"><a href="#seat-114"><span class="linenos">114</span></a>
-</span><span id="seat-115"><a href="#seat-115"><span class="linenos">115</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
-</span><span id="seat-116"><a href="#seat-116"><span class="linenos">116</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="seat-110"><a href="#seat-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">seat</span><span class="p">(</span>
+</span><span id="seat-111"><a href="#seat-111"><span class="linenos">111</span></a>    <span class="n">source</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">start_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">stop_line</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="seat-112"><a href="#seat-112"><span class="linenos">112</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="seat-113"><a href="#seat-113"><span class="linenos">113</span></a>    <span class="sd">&quot;&quot;&quot;Sort the contents of classes in `source`, where `source` is parsable Python code.</span>
+</span><span id="seat-114"><a href="#seat-114"><span class="linenos">114</span></a><span class="sd">    Anything not inside a class will be untouched.</span>
+</span><span id="seat-115"><a href="#seat-115"><span class="linenos">115</span></a>
+</span><span id="seat-116"><a href="#seat-116"><span class="linenos">116</span></a><span class="sd">    The modified `source` will be returned.</span>
 </span><span id="seat-117"><a href="#seat-117"><span class="linenos">117</span></a>
-</span><span id="seat-118"><a href="#seat-118"><span class="linenos">118</span></a><span class="sd">    #### :Sorting and Priority:</span>
+</span><span id="seat-118"><a href="#seat-118"><span class="linenos">118</span></a><span class="sd">    #### :params:</span>
 </span><span id="seat-119"><a href="#seat-119"><span class="linenos">119</span></a>
-</span><span id="seat-120"><a href="#seat-120"><span class="linenos">120</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
-</span><span id="seat-121"><a href="#seat-121"><span class="linenos">121</span></a><span class="sd">    * Dunder methods</span>
-</span><span id="seat-122"><a href="#seat-122"><span class="linenos">122</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
-</span><span id="seat-123"><a href="#seat-123"><span class="linenos">123</span></a><span class="sd">    * Class functions</span>
-</span><span id="seat-124"><a href="#seat-124"><span class="linenos">124</span></a>
-</span><span id="seat-125"><a href="#seat-125"><span class="linenos">125</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
+</span><span id="seat-120"><a href="#seat-120"><span class="linenos">120</span></a><span class="sd">    * `start_line`: Only sort contents after this line.</span>
+</span><span id="seat-121"><a href="#seat-121"><span class="linenos">121</span></a>
+</span><span id="seat-122"><a href="#seat-122"><span class="linenos">122</span></a><span class="sd">    * `stop_line`: Only sort contents before this line.</span>
+</span><span id="seat-123"><a href="#seat-123"><span class="linenos">123</span></a>
+</span><span id="seat-124"><a href="#seat-124"><span class="linenos">124</span></a><span class="sd">    If you have class contents that are grouped a certain way and you want the groups individually sorted</span>
+</span><span id="seat-125"><a href="#seat-125"><span class="linenos">125</span></a><span class="sd">    so that the grouping is maintained, you can use `# Seat` to demarcate the groups.</span>
 </span><span id="seat-126"><a href="#seat-126"><span class="linenos">126</span></a>
-</span><span id="seat-127"><a href="#seat-127"><span class="linenos">127</span></a><span class="sd">    The only exception is for dunder methods.</span>
-</span><span id="seat-128"><a href="#seat-128"><span class="linenos">128</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
-</span><span id="seat-129"><a href="#seat-129"><span class="linenos">129</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="seat-130"><a href="#seat-130"><span class="linenos">130</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="seat-131"><a href="#seat-131"><span class="linenos">131</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
-</span><span id="seat-132"><a href="#seat-132"><span class="linenos">132</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
-</span><span id="seat-133"><a href="#seat-133"><span class="linenos">133</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="seat-134"><a href="#seat-134"><span class="linenos">134</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
-</span><span id="seat-135"><a href="#seat-135"><span class="linenos">135</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
-</span><span id="seat-136"><a href="#seat-136"><span class="linenos">136</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
-</span><span id="seat-137"><a href="#seat-137"><span class="linenos">137</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Seats</span><span class="p">()</span>
-</span><span id="seat-138"><a href="#seat-138"><span class="linenos">138</span></a>                <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">child</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
-</span><span id="seat-139"><a href="#seat-139"><span class="linenos">139</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="seat-140"><a href="#seat-140"><span class="linenos">140</span></a>                        <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-141"><a href="#seat-141"><span class="linenos">141</span></a>                        <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
-</span><span id="seat-142"><a href="#seat-142"><span class="linenos">142</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-143"><a href="#seat-143"><span class="linenos">143</span></a>                        <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
-</span><span id="seat-144"><a href="#seat-144"><span class="linenos">144</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-145"><a href="#seat-145"><span class="linenos">145</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Expr</span><span class="p">:</span>
-</span><span id="seat-146"><a href="#seat-146"><span class="linenos">146</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">expressions</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
-</span><span id="seat-147"><a href="#seat-147"><span class="linenos">147</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
-</span><span id="seat-148"><a href="#seat-148"><span class="linenos">148</span></a>                            <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
-</span><span id="seat-149"><a href="#seat-149"><span class="linenos">149</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-150"><a href="#seat-150"><span class="linenos">150</span></a>                            <span class="k">else</span><span class="p">:</span>
-</span><span id="seat-151"><a href="#seat-151"><span class="linenos">151</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
-</span><span id="seat-152"><a href="#seat-152"><span class="linenos">152</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
-</span><span id="seat-153"><a href="#seat-153"><span class="linenos">153</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-154"><a href="#seat-154"><span class="linenos">154</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
-</span><span id="seat-155"><a href="#seat-155"><span class="linenos">155</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-156"><a href="#seat-156"><span class="linenos">156</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="seat-157"><a href="#seat-157"><span class="linenos">157</span></a>                            <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
-</span><span id="seat-158"><a href="#seat-158"><span class="linenos">158</span></a>                                <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
-</span><span id="seat-159"><a href="#seat-159"><span class="linenos">159</span></a>                                <span class="k">if</span> <span class="p">(</span>
-</span><span id="seat-160"><a href="#seat-160"><span class="linenos">160</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
-</span><span id="seat-161"><a href="#seat-161"><span class="linenos">161</span></a>                                    <span class="ow">and</span> <span class="s2">&quot;property&quot;</span> <span class="ow">in</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span>
-</span><span id="seat-162"><a href="#seat-162"><span class="linenos">162</span></a>                                <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
-</span><span id="seat-163"><a href="#seat-163"><span class="linenos">163</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
-</span><span id="seat-164"><a href="#seat-164"><span class="linenos">164</span></a>                                    <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
-</span><span id="seat-165"><a href="#seat-165"><span class="linenos">165</span></a>                                <span class="p">):</span>
-</span><span id="seat-166"><a href="#seat-166"><span class="linenos">166</span></a>                                    <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-167"><a href="#seat-167"><span class="linenos">167</span></a>                                    <span class="k">break</span>
-</span><span id="seat-168"><a href="#seat-168"><span class="linenos">168</span></a>                            <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
-</span><span id="seat-169"><a href="#seat-169"><span class="linenos">169</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-170"><a href="#seat-170"><span class="linenos">170</span></a>                        <span class="k">else</span><span class="p">:</span>
-</span><span id="seat-171"><a href="#seat-171"><span class="linenos">171</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
-</span><span id="seat-172"><a href="#seat-172"><span class="linenos">172</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="seat-173"><a href="#seat-173"><span class="linenos">173</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">child</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">))</span>
-</span><span id="seat-174"><a href="#seat-174"><span class="linenos">174</span></a>                        <span class="k">raise</span> <span class="n">e</span>
-</span><span id="seat-175"><a href="#seat-175"><span class="linenos">175</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
-</span><span id="seat-176"><a href="#seat-176"><span class="linenos">176</span></a>    <span class="k">return</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span>
+</span><span id="seat-127"><a href="#seat-127"><span class="linenos">127</span></a><span class="sd">    i.e. if the source is:</span>
+</span><span id="seat-128"><a href="#seat-128"><span class="linenos">128</span></a><span class="sd">    &gt;&gt;&gt; class MyClass():</span>
+</span><span id="seat-129"><a href="#seat-129"><span class="linenos">129</span></a><span class="sd">    &gt;&gt;&gt;     {arbitrary lines of code}</span>
+</span><span id="seat-130"><a href="#seat-130"><span class="linenos">130</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="seat-131"><a href="#seat-131"><span class="linenos">131</span></a><span class="sd">    &gt;&gt;&gt;     {more arbitrary code}</span>
+</span><span id="seat-132"><a href="#seat-132"><span class="linenos">132</span></a><span class="sd">    &gt;&gt;&gt;     # Seat</span>
+</span><span id="seat-133"><a href="#seat-133"><span class="linenos">133</span></a><span class="sd">    &gt;&gt;&gt;     {yet more code}</span>
+</span><span id="seat-134"><a href="#seat-134"><span class="linenos">134</span></a>
+</span><span id="seat-135"><a href="#seat-135"><span class="linenos">135</span></a><span class="sd">    Then the three sets of code in brackets will be sorted independently from one another</span>
+</span><span id="seat-136"><a href="#seat-136"><span class="linenos">136</span></a><span class="sd">    (assuming no values are given for `start_line` or `stop_line`).</span>
+</span><span id="seat-137"><a href="#seat-137"><span class="linenos">137</span></a>
+</span><span id="seat-138"><a href="#seat-138"><span class="linenos">138</span></a><span class="sd">    #### :Sorting and Priority:</span>
+</span><span id="seat-139"><a href="#seat-139"><span class="linenos">139</span></a>
+</span><span id="seat-140"><a href="#seat-140"><span class="linenos">140</span></a><span class="sd">    * Class variables declared in class body outside of a function</span>
+</span><span id="seat-141"><a href="#seat-141"><span class="linenos">141</span></a><span class="sd">    * Dunder methods</span>
+</span><span id="seat-142"><a href="#seat-142"><span class="linenos">142</span></a><span class="sd">    * Functions decorated with `property` or corresponding `.setter` and `.deleter` methods</span>
+</span><span id="seat-143"><a href="#seat-143"><span class="linenos">143</span></a><span class="sd">    * Class functions</span>
+</span><span id="seat-144"><a href="#seat-144"><span class="linenos">144</span></a>
+</span><span id="seat-145"><a href="#seat-145"><span class="linenos">145</span></a><span class="sd">    Each of these groups will be sorted alphabetically with respect to themselves.</span>
+</span><span id="seat-146"><a href="#seat-146"><span class="linenos">146</span></a>
+</span><span id="seat-147"><a href="#seat-147"><span class="linenos">147</span></a><span class="sd">    The only exception is for dunder methods.</span>
+</span><span id="seat-148"><a href="#seat-148"><span class="linenos">148</span></a><span class="sd">    They will be sorted alphabetically except that `__init__` will be first.</span>
+</span><span id="seat-149"><a href="#seat-149"><span class="linenos">149</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="seat-150"><a href="#seat-150"><span class="linenos">150</span></a>    <span class="n">tree</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="seat-151"><a href="#seat-151"><span class="linenos">151</span></a>    <span class="n">start_line</span> <span class="o">=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="mi">0</span>
+</span><span id="seat-152"><a href="#seat-152"><span class="linenos">152</span></a>    <span class="n">stop_line</span> <span class="o">=</span> <span class="n">stop_line</span> <span class="ow">or</span> <span class="nb">len</span><span class="p">(</span><span class="n">source</span><span class="o">.</span><span class="n">splitlines</span><span class="p">())</span> <span class="o">+</span> <span class="mi">1</span>
+</span><span id="seat-153"><a href="#seat-153"><span class="linenos">153</span></a>    <span class="n">sections</span> <span class="o">=</span> <span class="n">get_seat_sections</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="seat-154"><a href="#seat-154"><span class="linenos">154</span></a>    <span class="k">for</span> <span class="n">section</span> <span class="ow">in</span> <span class="n">sections</span><span class="p">:</span>
+</span><span id="seat-155"><a href="#seat-155"><span class="linenos">155</span></a>        <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">stmt</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="seat-156"><a href="#seat-156"><span class="linenos">156</span></a>            <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">stmt</span><span class="p">)</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ClassDef</span><span class="p">:</span>
+</span><span id="seat-157"><a href="#seat-157"><span class="linenos">157</span></a>                <span class="n">order</span> <span class="o">=</span> <span class="n">Seats</span><span class="p">()</span>
+</span><span id="seat-158"><a href="#seat-158"><span class="linenos">158</span></a>                <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">child</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">stmt</span><span class="o">.</span><span class="n">body</span><span class="p">):</span>
+</span><span id="seat-159"><a href="#seat-159"><span class="linenos">159</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="seat-160"><a href="#seat-160"><span class="linenos">160</span></a>                        <span class="n">type_</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-161"><a href="#seat-161"><span class="linenos">161</span></a>                        <span class="k">if</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;=</span> <span class="n">start_line</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&lt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
+</span><span id="seat-162"><a href="#seat-162"><span class="linenos">162</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">before</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-163"><a href="#seat-163"><span class="linenos">163</span></a>                        <span class="k">elif</span> <span class="n">stop_line</span> <span class="o">&lt;</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="ow">or</span> <span class="n">child</span><span class="o">.</span><span class="n">lineno</span> <span class="o">&gt;</span> <span class="n">section</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
+</span><span id="seat-164"><a href="#seat-164"><span class="linenos">164</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">after</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-165"><a href="#seat-165"><span class="linenos">165</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Expr</span><span class="p">:</span>
+</span><span id="seat-166"><a href="#seat-166"><span class="linenos">166</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">expressions</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="seat-167"><a href="#seat-167"><span class="linenos">167</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Comment</span><span class="p">:</span>
+</span><span id="seat-168"><a href="#seat-168"><span class="linenos">168</span></a>                            <span class="k">if</span> <span class="s2">&quot;# Seat&quot;</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">value</span><span class="p">:</span>
+</span><span id="seat-169"><a href="#seat-169"><span class="linenos">169</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">seats</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-170"><a href="#seat-170"><span class="linenos">170</span></a>                            <span class="k">else</span><span class="p">:</span>
+</span><span id="seat-171"><a href="#seat-171"><span class="linenos">171</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">comments</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">child</span><span class="p">,</span> <span class="n">j</span><span class="p">))</span>
+</span><span id="seat-172"><a href="#seat-172"><span class="linenos">172</span></a>                        <span class="k">elif</span> <span class="n">type_</span> <span class="ow">in</span> <span class="p">[</span><span class="n">ast</span><span class="o">.</span><span class="n">Assign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AugAssign</span><span class="p">,</span> <span class="n">ast</span><span class="o">.</span><span class="n">AnnAssign</span><span class="p">]:</span>
+</span><span id="seat-173"><a href="#seat-173"><span class="linenos">173</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">assigns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-174"><a href="#seat-174"><span class="linenos">174</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">)</span> <span class="ow">and</span> <span class="n">child</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;__&quot;</span><span class="p">):</span>
+</span><span id="seat-175"><a href="#seat-175"><span class="linenos">175</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">dunders</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-176"><a href="#seat-176"><span class="linenos">176</span></a>                        <span class="k">elif</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="seat-177"><a href="#seat-177"><span class="linenos">177</span></a>                            <span class="k">for</span> <span class="n">decorator</span> <span class="ow">in</span> <span class="n">child</span><span class="o">.</span><span class="n">decorator_list</span><span class="p">:</span>
+</span><span id="seat-178"><a href="#seat-178"><span class="linenos">178</span></a>                                <span class="n">decorator_type</span> <span class="o">=</span> <span class="nb">type</span><span class="p">(</span><span class="n">decorator</span><span class="p">)</span>
+</span><span id="seat-179"><a href="#seat-179"><span class="linenos">179</span></a>                                <span class="k">if</span> <span class="p">(</span>
+</span><span id="seat-180"><a href="#seat-180"><span class="linenos">180</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Name</span>
+</span><span id="seat-181"><a href="#seat-181"><span class="linenos">181</span></a>                                    <span class="ow">and</span> <span class="s2">&quot;property&quot;</span> <span class="ow">in</span> <span class="n">decorator</span><span class="o">.</span><span class="n">id</span>
+</span><span id="seat-182"><a href="#seat-182"><span class="linenos">182</span></a>                                <span class="p">)</span> <span class="ow">or</span> <span class="p">(</span>
+</span><span id="seat-183"><a href="#seat-183"><span class="linenos">183</span></a>                                    <span class="n">decorator_type</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">Attribute</span>
+</span><span id="seat-184"><a href="#seat-184"><span class="linenos">184</span></a>                                    <span class="ow">and</span> <span class="n">decorator</span><span class="o">.</span><span class="n">attr</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;setter&quot;</span><span class="p">,</span> <span class="s2">&quot;deleter&quot;</span><span class="p">]</span>
+</span><span id="seat-185"><a href="#seat-185"><span class="linenos">185</span></a>                                <span class="p">):</span>
+</span><span id="seat-186"><a href="#seat-186"><span class="linenos">186</span></a>                                    <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-187"><a href="#seat-187"><span class="linenos">187</span></a>                                    <span class="k">break</span>
+</span><span id="seat-188"><a href="#seat-188"><span class="linenos">188</span></a>                            <span class="k">if</span> <span class="n">child</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">order</span><span class="o">.</span><span class="n">properties</span><span class="p">:</span>
+</span><span id="seat-189"><a href="#seat-189"><span class="linenos">189</span></a>                                <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-190"><a href="#seat-190"><span class="linenos">190</span></a>                        <span class="k">else</span><span class="p">:</span>
+</span><span id="seat-191"><a href="#seat-191"><span class="linenos">191</span></a>                            <span class="n">order</span><span class="o">.</span><span class="n">functions</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">child</span><span class="p">)</span>
+</span><span id="seat-192"><a href="#seat-192"><span class="linenos">192</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="seat-193"><a href="#seat-193"><span class="linenos">193</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">child</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">))</span>
+</span><span id="seat-194"><a href="#seat-194"><span class="linenos">194</span></a>                        <span class="k">raise</span> <span class="n">e</span>
+</span><span id="seat-195"><a href="#seat-195"><span class="linenos">195</span></a>                <span class="n">tree</span><span class="o">.</span><span class="n">body</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">body</span> <span class="o">=</span> <span class="n">order</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
+</span><span id="seat-196"><a href="#seat-196"><span class="linenos">196</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">ast</span><span class="o">.</span><span class="n">unparse</span><span class="p">(</span><span class="n">tree</span><span class="p">)</span>
+</span><span id="seat-197"><a href="#seat-197"><span class="linenos">197</span></a>    <span class="k">return</span> <span class="n">fix_type_ignore</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sort the contents of classes in <code>source</code>, where <code>source</code> is parsable Python code.
 Anything not inside a class will be untouched.</p>
 
 <p>The modified <code>source</code> will be returned.</p>
@@ -737,52 +814,52 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-179"><a href="#get_args-179"><span class="linenos">179</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-180"><a href="#get_args-180"><span class="linenos">180</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-181"><a href="#get_args-181"><span class="linenos">181</span></a>
-</span><span id="get_args-182"><a href="#get_args-182"><span class="linenos">182</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
-</span><span id="get_args-183"><a href="#get_args-183"><span class="linenos">183</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-184"><a href="#get_args-184"><span class="linenos">184</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
-</span><span id="get_args-185"><a href="#get_args-185"><span class="linenos">185</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
-</span><span id="get_args-186"><a href="#get_args-186"><span class="linenos">186</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-187"><a href="#get_args-187"><span class="linenos">187</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-188"><a href="#get_args-188"><span class="linenos">188</span></a>    <span class="p">)</span>
-</span><span id="get_args-189"><a href="#get_args-189"><span class="linenos">189</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-190"><a href="#get_args-190"><span class="linenos">190</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
-</span><span id="get_args-191"><a href="#get_args-191"><span class="linenos">191</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
-</span><span id="get_args-192"><a href="#get_args-192"><span class="linenos">192</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-193"><a href="#get_args-193"><span class="linenos">193</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-194"><a href="#get_args-194"><span class="linenos">194</span></a>    <span class="p">)</span>
-</span><span id="get_args-195"><a href="#get_args-195"><span class="linenos">195</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-196"><a href="#get_args-196"><span class="linenos">196</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
-</span><span id="get_args-197"><a href="#get_args-197"><span class="linenos">197</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
-</span><span id="get_args-198"><a href="#get_args-198"><span class="linenos">198</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-199"><a href="#get_args-199"><span class="linenos">199</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-200"><a href="#get_args-200"><span class="linenos">200</span></a>    <span class="p">)</span>
-</span><span id="get_args-201"><a href="#get_args-201"><span class="linenos">201</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-202"><a href="#get_args-202"><span class="linenos">202</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="get_args-203"><a href="#get_args-203"><span class="linenos">203</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
-</span><span id="get_args-204"><a href="#get_args-204"><span class="linenos">204</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="get_args-205"><a href="#get_args-205"><span class="linenos">205</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-206"><a href="#get_args-206"><span class="linenos">206</span></a>    <span class="p">)</span>
-</span><span id="get_args-207"><a href="#get_args-207"><span class="linenos">207</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-208"><a href="#get_args-208"><span class="linenos">208</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="get_args-209"><a href="#get_args-209"><span class="linenos">209</span></a>        <span class="s2">&quot;--dump&quot;</span><span class="p">,</span>
-</span><span id="get_args-210"><a href="#get_args-210"><span class="linenos">210</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-211"><a href="#get_args-211"><span class="linenos">211</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Dump ast tree to file instead of doing anything else. </span>
-</span><span id="get_args-212"><a href="#get_args-212"><span class="linenos">212</span></a><span class="s2">        For debugging purposes.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-213"><a href="#get_args-213"><span class="linenos">213</span></a>    <span class="p">)</span>
-</span><span id="get_args-214"><a href="#get_args-214"><span class="linenos">214</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-215"><a href="#get_args-215"><span class="linenos">215</span></a>
-</span><span id="get_args-216"><a href="#get_args-216"><span class="linenos">216</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-200"><a href="#get_args-200"><span class="linenos">200</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-201"><a href="#get_args-201"><span class="linenos">201</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-202"><a href="#get_args-202"><span class="linenos">202</span></a>
+</span><span id="get_args-203"><a href="#get_args-203"><span class="linenos">203</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The file to format. &quot;&quot;&quot;</span><span class="p">)</span>
+</span><span id="get_args-204"><a href="#get_args-204"><span class="linenos">204</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-205"><a href="#get_args-205"><span class="linenos">205</span></a>        <span class="s2">&quot;--start&quot;</span><span class="p">,</span>
+</span><span id="get_args-206"><a href="#get_args-206"><span class="linenos">206</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
+</span><span id="get_args-207"><a href="#get_args-207"><span class="linenos">207</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-208"><a href="#get_args-208"><span class="linenos">208</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to start formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-209"><a href="#get_args-209"><span class="linenos">209</span></a>    <span class="p">)</span>
+</span><span id="get_args-210"><a href="#get_args-210"><span class="linenos">210</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-211"><a href="#get_args-211"><span class="linenos">211</span></a>        <span class="s2">&quot;--stop&quot;</span><span class="p">,</span>
+</span><span id="get_args-212"><a href="#get_args-212"><span class="linenos">212</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">int</span><span class="p">,</span>
+</span><span id="get_args-213"><a href="#get_args-213"><span class="linenos">213</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-214"><a href="#get_args-214"><span class="linenos">214</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Optional line number to stop formatting at. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-215"><a href="#get_args-215"><span class="linenos">215</span></a>    <span class="p">)</span>
+</span><span id="get_args-216"><a href="#get_args-216"><span class="linenos">216</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-217"><a href="#get_args-217"><span class="linenos">217</span></a>        <span class="s2">&quot;-nb&quot;</span><span class="p">,</span>
+</span><span id="get_args-218"><a href="#get_args-218"><span class="linenos">218</span></a>        <span class="s2">&quot;--noblack&quot;</span><span class="p">,</span>
+</span><span id="get_args-219"><a href="#get_args-219"><span class="linenos">219</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-220"><a href="#get_args-220"><span class="linenos">220</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t format file with Black after sorting. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-221"><a href="#get_args-221"><span class="linenos">221</span></a>    <span class="p">)</span>
+</span><span id="get_args-222"><a href="#get_args-222"><span class="linenos">222</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-223"><a href="#get_args-223"><span class="linenos">223</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="get_args-224"><a href="#get_args-224"><span class="linenos">224</span></a>        <span class="s2">&quot;--output&quot;</span><span class="p">,</span>
+</span><span id="get_args-225"><a href="#get_args-225"><span class="linenos">225</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="get_args-226"><a href="#get_args-226"><span class="linenos">226</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Write changes to this file, otherwise changes are written back to the original file. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-227"><a href="#get_args-227"><span class="linenos">227</span></a>    <span class="p">)</span>
+</span><span id="get_args-228"><a href="#get_args-228"><span class="linenos">228</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-229"><a href="#get_args-229"><span class="linenos">229</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="get_args-230"><a href="#get_args-230"><span class="linenos">230</span></a>        <span class="s2">&quot;--dump&quot;</span><span class="p">,</span>
+</span><span id="get_args-231"><a href="#get_args-231"><span class="linenos">231</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-232"><a href="#get_args-232"><span class="linenos">232</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Dump ast tree to file instead of doing anything else. </span>
+</span><span id="get_args-233"><a href="#get_args-233"><span class="linenos">233</span></a><span class="s2">        For debugging purposes.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-234"><a href="#get_args-234"><span class="linenos">234</span></a>    <span class="p">)</span>
+</span><span id="get_args-235"><a href="#get_args-235"><span class="linenos">235</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-236"><a href="#get_args-236"><span class="linenos">236</span></a>
+</span><span id="get_args-237"><a href="#get_args-237"><span class="linenos">237</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="main">
@@ -792,28 +869,28 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">dump</span><span class="p">:</span>
-</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span>
-</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_ast_dump.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>            <span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
-</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>        <span class="p">)</span>
-</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
-</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
-</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>            <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
-</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>    <span class="n">source</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">dump</span><span class="p">:</span>
+</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span>
+</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>        <span class="n">file</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_ast_dump.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>            <span class="n">ast</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">ast</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">type_comments</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="n">indent</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
+</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>        <span class="p">)</span>
+</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">seat</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">start</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">stop</span><span class="p">)</span>
+</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">noblack</span><span class="p">:</span>
+</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>            <span class="n">source</span> <span class="o">=</span> <span class="n">black</span><span class="o">.</span><span class="n">format_str</span><span class="p">(</span><span class="n">source</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="n">black</span><span class="o">.</span><span class="n">Mode</span><span class="p">())</span>
+</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">output</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -6,14 +6,15 @@
     * get_seat_sections
     * Seats
           o Seats
           o sort_nodes_by_name
           o sort_dunders
           o sort_assigns
           o sort
+    * fix_type_ignore
     * seat
     * get_args
     * main
 built_with_pdoc[pdoc_logo]
 
 ****** seating.seating ******
 ⁰ View Source
@@ -105,173 +106,194 @@
 _82            + self.after
 _83        )
 _84        for expression in self.expressions + self.comments:
 _85            body.insert(expression[1], expression[0])
 _86        return body
 _87
 _88
-_89def seat(
-_90    source: str, start_line: int | None = None, stop_line: int | None = None
-_91) -> str:
-_92    """Sort the contents of classes in `source`, where `source` is parsable
-Python code.
-_93    Anything not inside a class will be untouched.
+_89def fix_type_ignore(source: str) -> str:
+_90    """Fix misplacement of `# type: ignore` comments in sorted `source`.
+_91
+_92    Corrects when
+_93    >>> var = 6 # type: ignore
 _94
-_95    The modified `source` will be returned.
+_95    gets turned into
 _96
-_97    #### :params:
-_98
-_99    * `start_line`: Only sort contents after this line.
-100
-101    * `stop_line`: Only sort contents before this line.
-102
-103    If you have class contents that are grouped a certain way and you want
+_97    >>> # type: ignore
+_98    >>> var = 6"""
+_99    lines = source.splitlines(True)
+100    clean = lambda s: s.replace(" ", "").replace("\n", "")
+101    for i, line in enumerate(lines):
+102        if clean(line) == "#type:ignore" and 0 < i < len(lines):
+103            lines[i] = ""
+104            if "#type:ignore" not in clean(lines[i + 1]):
+105                lines[i + 1] = lines[i + 1].strip("\n") + "# type: ignore\n"
+106    return "".join(lines)
+107
+108
+109def seat(
+110    source: str, start_line: int | None = None, stop_line: int | None = None
+111) -> str:
+112    """Sort the contents of classes in `source`, where `source` is parsable
+Python code.
+113    Anything not inside a class will be untouched.
+114
+115    The modified `source` will be returned.
+116
+117    #### :params:
+118
+119    * `start_line`: Only sort contents after this line.
+120
+121    * `stop_line`: Only sort contents before this line.
+122
+123    If you have class contents that are grouped a certain way and you want
 the groups individually sorted
-104    so that the grouping is maintained, you can use `# Seat` to demarcate
+124    so that the grouping is maintained, you can use `# Seat` to demarcate
 the groups.
-105
-106    i.e. if the source is:
-107    >>> class MyClass():
-108    >>>     {arbitrary lines of code}
-109    >>>     # Seat
-110    >>>     {more arbitrary code}
-111    >>>     # Seat
-112    >>>     {yet more code}
-113
-114    Then the three sets of code in brackets will be sorted independently
+125
+126    i.e. if the source is:
+127    >>> class MyClass():
+128    >>>     {arbitrary lines of code}
+129    >>>     # Seat
+130    >>>     {more arbitrary code}
+131    >>>     # Seat
+132    >>>     {yet more code}
+133
+134    Then the three sets of code in brackets will be sorted independently
 from one another
-115    (assuming no values are given for `start_line` or `stop_line`).
-116
-117    #### :Sorting and Priority:
-118
-119    * Class variables declared in class body outside of a function
-120    * Dunder methods
-121    * Functions decorated with `property` or corresponding `.setter` and
+135    (assuming no values are given for `start_line` or `stop_line`).
+136
+137    #### :Sorting and Priority:
+138
+139    * Class variables declared in class body outside of a function
+140    * Dunder methods
+141    * Functions decorated with `property` or corresponding `.setter` and
 `.deleter` methods
-122    * Class functions
-123
-124    Each of these groups will be sorted alphabetically with respect to
+142    * Class functions
+143
+144    Each of these groups will be sorted alphabetically with respect to
 themselves.
-125
-126    The only exception is for dunder methods.
-127    They will be sorted alphabetically except that `__init__` will be first.
-128    """
-129    tree = ast.parse(source, type_comments=True)
-130    start_line = start_line or 0
-131    stop_line = stop_line or len(source.splitlines()) + 1
-132    sections = get_seat_sections(source)
-133    for section in sections:
-134        for i, stmt in enumerate(tree.body):
-135            if type(stmt) == ast.ClassDef:
-136                order = Seats()
-137                for j, child in enumerate(stmt.body):
-138                    try:
-139                        type_ = type(child)
-140                        if child.lineno <= start_line or child.lineno <
+145
+146    The only exception is for dunder methods.
+147    They will be sorted alphabetically except that `__init__` will be first.
+148    """
+149    tree = ast.parse(source, type_comments=True)
+150    start_line = start_line or 0
+151    stop_line = stop_line or len(source.splitlines()) + 1
+152    sections = get_seat_sections(source)
+153    for section in sections:
+154        for i, stmt in enumerate(tree.body):
+155            if type(stmt) == ast.ClassDef:
+156                order = Seats()
+157                for j, child in enumerate(stmt.body):
+158                    try:
+159                        type_ = type(child)
+160                        if child.lineno <= start_line or child.lineno <
 section[0]:
-141                            order.before.append(child)
-142                        elif stop_line < child.lineno or child.lineno >
+161                            order.before.append(child)
+162                        elif stop_line < child.lineno or child.lineno >
 section[1]:
-143                            order.after.append(child)
-144                        elif type_ == ast.Expr:
-145                            order.expressions.append((child, j))
-146                        elif type_ == ast.Comment:
-147                            if "# Seat" in child.value:
-148                                order.seats.append(child)
-149                            else:
-150                                order.comments.append((child, j))
-151                        elif type_ in [ast.Assign, ast.AugAssign,
+163                            order.after.append(child)
+164                        elif type_ == ast.Expr:
+165                            order.expressions.append((child, j))
+166                        elif type_ == ast.Comment:
+167                            if "# Seat" in child.value:
+168                                order.seats.append(child)
+169                            else:
+170                                order.comments.append((child, j))
+171                        elif type_ in [ast.Assign, ast.AugAssign,
 ast.AnnAssign]:
-152                            order.assigns.append(child)
-153                        elif child.name.startswith("__") and
+172                            order.assigns.append(child)
+173                        elif child.name.startswith("__") and
 child.name.endswith("__"):
-154                            order.dunders.append(child)
-155                        elif child.decorator_list:
-156                            for decorator in child.decorator_list:
-157                                decorator_type = type(decorator)
-158                                if (
-159                                    decorator_type == ast.Name
-160                                    and "property" in decorator.id
-161                                ) or (
-162                                    decorator_type == ast.Attribute
-163                                    and decorator.attr in ["setter",
+174                            order.dunders.append(child)
+175                        elif child.decorator_list:
+176                            for decorator in child.decorator_list:
+177                                decorator_type = type(decorator)
+178                                if (
+179                                    decorator_type == ast.Name
+180                                    and "property" in decorator.id
+181                                ) or (
+182                                    decorator_type == ast.Attribute
+183                                    and decorator.attr in ["setter",
 "deleter"]
-164                                ):
-165                                    order.properties.append(child)
-166                                    break
-167                            if child not in order.properties:
-168                                order.functions.append(child)
-169                        else:
-170                            order.functions.append(child)
-171                    except Exception as e:
-172                        print(ast.dump(child, indent=2))
-173                        raise e
-174                tree.body[i].body = order.sort()
-175    return ast.unparse(tree)
-176
-177
-178def get_args() -> argparse.Namespace:
-179    parser = argparse.ArgumentParser()
-180
-181    parser.add_argument("file", type=str, help=""" The file to format. """)
-182    parser.add_argument(
-183        "--start",
-184        type=int,
-185        default=None,
-186        help=""" Optional line number to start formatting at. """,
-187    )
-188    parser.add_argument(
-189        "--stop",
-190        type=int,
-191        default=None,
-192        help=""" Optional line number to stop formatting at. """,
-193    )
-194    parser.add_argument(
-195        "-nb",
-196        "--noblack",
-197        action="store_true",
-198        help=""" Don't format file with Black after sorting. """,
-199    )
-200    parser.add_argument(
-201        "-o",
-202        "--output",
-203        default=None,
-204        help=""" Write changes to this file, otherwise changes are written
+184                                ):
+185                                    order.properties.append(child)
+186                                    break
+187                            if child not in order.properties:
+188                                order.functions.append(child)
+189                        else:
+190                            order.functions.append(child)
+191                    except Exception as e:
+192                        print(ast.dump(child, indent=2))
+193                        raise e
+194                tree.body[i].body = order.sort()
+195    source = ast.unparse(tree)
+196    return fix_type_ignore(source)
+197
+198
+199def get_args() -> argparse.Namespace:
+200    parser = argparse.ArgumentParser()
+201
+202    parser.add_argument("file", type=str, help=""" The file to format. """)
+203    parser.add_argument(
+204        "--start",
+205        type=int,
+206        default=None,
+207        help=""" Optional line number to start formatting at. """,
+208    )
+209    parser.add_argument(
+210        "--stop",
+211        type=int,
+212        default=None,
+213        help=""" Optional line number to stop formatting at. """,
+214    )
+215    parser.add_argument(
+216        "-nb",
+217        "--noblack",
+218        action="store_true",
+219        help=""" Don't format file with Black after sorting. """,
+220    )
+221    parser.add_argument(
+222        "-o",
+223        "--output",
+224        default=None,
+225        help=""" Write changes to this file, otherwise changes are written
 back to the original file. """,
-205    )
-206    parser.add_argument(
-207        "-d",
-208        "--dump",
-209        action="store_true",
-210        help=""" Dump ast tree to file instead of doing anything else.
-211        For debugging purposes.""",
-212    )
-213    args = parser.parse_args()
-214
-215    return args
-216
-217
-218def main(args: argparse.Namespace | None = None):
-219    if not args:
-220        args = get_args()
-221    source = Pathier(args.file).read_text()
-222    if args.dump:
-223        file = Pathier(args.file)
-224        file = file.with_name(f"{file.stem}_ast_dump.txt").write_text(
-225            ast.dump(ast.parse(source, type_comments=True), indent=2)
-226        )
-227    else:
-228        source = seat(source, args.start, args.stop)
-229        if not args.noblack:
-230            source = black.format_str(source, mode=black.Mode())
-231        Pathier(args.output or args.file).write_text(source)
-232
-233
-234if __name__ == "__main__":
-235    main(get_args())
+226    )
+227    parser.add_argument(
+228        "-d",
+229        "--dump",
+230        action="store_true",
+231        help=""" Dump ast tree to file instead of doing anything else.
+232        For debugging purposes.""",
+233    )
+234    args = parser.parse_args()
+235
+236    return args
+237
+238
+239def main(args: argparse.Namespace | None = None):
+240    if not args:
+241        args = get_args()
+242    source = Pathier(args.file).read_text()
+243    if args.dump:
+244        file = Pathier(args.file)
+245        file = file.with_name(f"{file.stem}_ast_dump.txt").write_text(
+246            ast.dump(ast.parse(source, type_comments=True), indent=2)
+247        )
+248    else:
+249        source = seat(source, args.start, args.stop)
+250        if not args.noblack:
+251            source = black.format_str(source, mode=black.Mode())
+252        Pathier(args.output or args.file).write_text(source)
+253
+254
+255if __name__ == "__main__":
+256    main(get_args())
   ⁰
 def get_seat_sections(source: str) -> list[tuple[int, int]]: View Source
 _9def get_seat_sections(source: str) -> list[tuple[int, int]]:
 10    """Return a list of line number pairs for content between `# Seat`
 comments in `source`.
 11
 12    If `source` has no `# Seat` comments, a list with one tuple will be
@@ -425,116 +447,143 @@
 83            + self.after
 84        )
 85        for expression in self.expressions + self.comments:
 86            body.insert(expression[1], expression[0])
 87        return body
 Sort and return members as a single list.
   ⁰
+def fix_type_ignore(source: str) -> str: View Source
+_90def fix_type_ignore(source: str) -> str:
+_91    """Fix misplacement of `# type: ignore` comments in sorted `source`.
+_92
+_93    Corrects when
+_94    >>> var = 6 # type: ignore
+_95
+_96    gets turned into
+_97
+_98    >>> # type: ignore
+_99    >>> var = 6"""
+100    lines = source.splitlines(True)
+101    clean = lambda s: s.replace(" ", "").replace("\n", "")
+102    for i, line in enumerate(lines):
+103        if clean(line) == "#type:ignore" and 0 < i < len(lines):
+104            lines[i] = ""
+105            if "#type:ignore" not in clean(lines[i + 1]):
+106                lines[i + 1] = lines[i + 1].strip("\n") + "# type: ignore\n"
+107    return "".join(lines)
+Fix misplacement of # type: ignore comments in sorted source.
+Corrects when
+>>> var = 6 # type: ignore
+gets turned into
+>>> # type: ignore
+>>> var = 6
+  ⁰
 def seat(
 source: str,
 start_line: int | None = None,
 stop_line: int | None = None) -> str: View Source
-_90def seat(
-_91    source: str, start_line: int | None = None, stop_line: int | None = None
-_92) -> str:
-_93    """Sort the contents of classes in `source`, where `source` is parsable
+110def seat(
+111    source: str, start_line: int | None = None, stop_line: int | None = None
+112) -> str:
+113    """Sort the contents of classes in `source`, where `source` is parsable
 Python code.
-_94    Anything not inside a class will be untouched.
-_95
-_96    The modified `source` will be returned.
-_97
-_98    #### :params:
-_99
-100    * `start_line`: Only sort contents after this line.
-101
-102    * `stop_line`: Only sort contents before this line.
-103
-104    If you have class contents that are grouped a certain way and you want
+114    Anything not inside a class will be untouched.
+115
+116    The modified `source` will be returned.
+117
+118    #### :params:
+119
+120    * `start_line`: Only sort contents after this line.
+121
+122    * `stop_line`: Only sort contents before this line.
+123
+124    If you have class contents that are grouped a certain way and you want
 the groups individually sorted
-105    so that the grouping is maintained, you can use `# Seat` to demarcate
+125    so that the grouping is maintained, you can use `# Seat` to demarcate
 the groups.
-106
-107    i.e. if the source is:
-108    >>> class MyClass():
-109    >>>     {arbitrary lines of code}
-110    >>>     # Seat
-111    >>>     {more arbitrary code}
-112    >>>     # Seat
-113    >>>     {yet more code}
-114
-115    Then the three sets of code in brackets will be sorted independently
+126
+127    i.e. if the source is:
+128    >>> class MyClass():
+129    >>>     {arbitrary lines of code}
+130    >>>     # Seat
+131    >>>     {more arbitrary code}
+132    >>>     # Seat
+133    >>>     {yet more code}
+134
+135    Then the three sets of code in brackets will be sorted independently
 from one another
-116    (assuming no values are given for `start_line` or `stop_line`).
-117
-118    #### :Sorting and Priority:
-119
-120    * Class variables declared in class body outside of a function
-121    * Dunder methods
-122    * Functions decorated with `property` or corresponding `.setter` and
+136    (assuming no values are given for `start_line` or `stop_line`).
+137
+138    #### :Sorting and Priority:
+139
+140    * Class variables declared in class body outside of a function
+141    * Dunder methods
+142    * Functions decorated with `property` or corresponding `.setter` and
 `.deleter` methods
-123    * Class functions
-124
-125    Each of these groups will be sorted alphabetically with respect to
+143    * Class functions
+144
+145    Each of these groups will be sorted alphabetically with respect to
 themselves.
-126
-127    The only exception is for dunder methods.
-128    They will be sorted alphabetically except that `__init__` will be first.
-129    """
-130    tree = ast.parse(source, type_comments=True)
-131    start_line = start_line or 0
-132    stop_line = stop_line or len(source.splitlines()) + 1
-133    sections = get_seat_sections(source)
-134    for section in sections:
-135        for i, stmt in enumerate(tree.body):
-136            if type(stmt) == ast.ClassDef:
-137                order = Seats()
-138                for j, child in enumerate(stmt.body):
-139                    try:
-140                        type_ = type(child)
-141                        if child.lineno <= start_line or child.lineno <
+146
+147    The only exception is for dunder methods.
+148    They will be sorted alphabetically except that `__init__` will be first.
+149    """
+150    tree = ast.parse(source, type_comments=True)
+151    start_line = start_line or 0
+152    stop_line = stop_line or len(source.splitlines()) + 1
+153    sections = get_seat_sections(source)
+154    for section in sections:
+155        for i, stmt in enumerate(tree.body):
+156            if type(stmt) == ast.ClassDef:
+157                order = Seats()
+158                for j, child in enumerate(stmt.body):
+159                    try:
+160                        type_ = type(child)
+161                        if child.lineno <= start_line or child.lineno <
 section[0]:
-142                            order.before.append(child)
-143                        elif stop_line < child.lineno or child.lineno >
+162                            order.before.append(child)
+163                        elif stop_line < child.lineno or child.lineno >
 section[1]:
-144                            order.after.append(child)
-145                        elif type_ == ast.Expr:
-146                            order.expressions.append((child, j))
-147                        elif type_ == ast.Comment:
-148                            if "# Seat" in child.value:
-149                                order.seats.append(child)
-150                            else:
-151                                order.comments.append((child, j))
-152                        elif type_ in [ast.Assign, ast.AugAssign,
+164                            order.after.append(child)
+165                        elif type_ == ast.Expr:
+166                            order.expressions.append((child, j))
+167                        elif type_ == ast.Comment:
+168                            if "# Seat" in child.value:
+169                                order.seats.append(child)
+170                            else:
+171                                order.comments.append((child, j))
+172                        elif type_ in [ast.Assign, ast.AugAssign,
 ast.AnnAssign]:
-153                            order.assigns.append(child)
-154                        elif child.name.startswith("__") and
+173                            order.assigns.append(child)
+174                        elif child.name.startswith("__") and
 child.name.endswith("__"):
-155                            order.dunders.append(child)
-156                        elif child.decorator_list:
-157                            for decorator in child.decorator_list:
-158                                decorator_type = type(decorator)
-159                                if (
-160                                    decorator_type == ast.Name
-161                                    and "property" in decorator.id
-162                                ) or (
-163                                    decorator_type == ast.Attribute
-164                                    and decorator.attr in ["setter",
+175                            order.dunders.append(child)
+176                        elif child.decorator_list:
+177                            for decorator in child.decorator_list:
+178                                decorator_type = type(decorator)
+179                                if (
+180                                    decorator_type == ast.Name
+181                                    and "property" in decorator.id
+182                                ) or (
+183                                    decorator_type == ast.Attribute
+184                                    and decorator.attr in ["setter",
 "deleter"]
-165                                ):
-166                                    order.properties.append(child)
-167                                    break
-168                            if child not in order.properties:
-169                                order.functions.append(child)
-170                        else:
-171                            order.functions.append(child)
-172                    except Exception as e:
-173                        print(ast.dump(child, indent=2))
-174                        raise e
-175                tree.body[i].body = order.sort()
-176    return ast.unparse(tree)
+185                                ):
+186                                    order.properties.append(child)
+187                                    break
+188                            if child not in order.properties:
+189                                order.functions.append(child)
+190                        else:
+191                            order.functions.append(child)
+192                    except Exception as e:
+193                        print(ast.dump(child, indent=2))
+194                        raise e
+195                tree.body[i].body = order.sort()
+196    source = ast.unparse(tree)
+197    return fix_type_ignore(source)
 Sort the contents of classes in source, where source is parsable Python code.
 Anything not inside a class will be untouched.
 The modified source will be returned.
 *** :params: ***
     * start_line: Only sort contents after this line.
     * stop_line: Only sort contents before this line.
 If you have class contents that are grouped a certain way and you want the
@@ -556,63 +605,63 @@
       methods
     * Class functions
 Each of these groups will be sorted alphabetically with respect to themselves.
 The only exception is for dunder methods. They will be sorted alphabetically
 except that __init__ will be first.
   ⁰
 def get_args() -> argparse.Namespace: View Source
-179def get_args() -> argparse.Namespace:
-180    parser = argparse.ArgumentParser()
-181
-182    parser.add_argument("file", type=str, help=""" The file to format. """)
-183    parser.add_argument(
-184        "--start",
-185        type=int,
-186        default=None,
-187        help=""" Optional line number to start formatting at. """,
-188    )
-189    parser.add_argument(
-190        "--stop",
-191        type=int,
-192        default=None,
-193        help=""" Optional line number to stop formatting at. """,
-194    )
-195    parser.add_argument(
-196        "-nb",
-197        "--noblack",
-198        action="store_true",
-199        help=""" Don't format file with Black after sorting. """,
-200    )
-201    parser.add_argument(
-202        "-o",
-203        "--output",
-204        default=None,
-205        help=""" Write changes to this file, otherwise changes are written
+200def get_args() -> argparse.Namespace:
+201    parser = argparse.ArgumentParser()
+202
+203    parser.add_argument("file", type=str, help=""" The file to format. """)
+204    parser.add_argument(
+205        "--start",
+206        type=int,
+207        default=None,
+208        help=""" Optional line number to start formatting at. """,
+209    )
+210    parser.add_argument(
+211        "--stop",
+212        type=int,
+213        default=None,
+214        help=""" Optional line number to stop formatting at. """,
+215    )
+216    parser.add_argument(
+217        "-nb",
+218        "--noblack",
+219        action="store_true",
+220        help=""" Don't format file with Black after sorting. """,
+221    )
+222    parser.add_argument(
+223        "-o",
+224        "--output",
+225        default=None,
+226        help=""" Write changes to this file, otherwise changes are written
 back to the original file. """,
-206    )
-207    parser.add_argument(
-208        "-d",
-209        "--dump",
-210        action="store_true",
-211        help=""" Dump ast tree to file instead of doing anything else.
-212        For debugging purposes.""",
-213    )
-214    args = parser.parse_args()
-215
-216    return args
+227    )
+228    parser.add_argument(
+229        "-d",
+230        "--dump",
+231        action="store_true",
+232        help=""" Dump ast tree to file instead of doing anything else.
+233        For debugging purposes.""",
+234    )
+235    args = parser.parse_args()
+236
+237    return args
   ⁰
 def main(args: argparse.Namespace | None = None): View Source
-219def main(args: argparse.Namespace | None = None):
-220    if not args:
-221        args = get_args()
-222    source = Pathier(args.file).read_text()
-223    if args.dump:
-224        file = Pathier(args.file)
-225        file = file.with_name(f"{file.stem}_ast_dump.txt").write_text(
-226            ast.dump(ast.parse(source, type_comments=True), indent=2)
-227        )
-228    else:
-229        source = seat(source, args.start, args.stop)
-230        if not args.noblack:
-231            source = black.format_str(source, mode=black.Mode())
-232        Pathier(args.output or args.file).write_text(source)
+240def main(args: argparse.Namespace | None = None):
+241    if not args:
+242        args = get_args()
+243    source = Pathier(args.file).read_text()
+244    if args.dump:
+245        file = Pathier(args.file)
+246        file = file.with_name(f"{file.stem}_ast_dump.txt").write_text(
+247            ast.dump(ast.parse(source, type_comments=True), indent=2)
+248        )
+249    else:
+250        source = seat(source, args.start, args.stop)
+251        if not args.noblack:
+252            source = black.format_str(source, mode=black.Mode())
+253        Pathier(args.output or args.file).write_text(source)
```

### Comparing `seating-0.0.1/src/seating/seating.py` & `seating-0.0.2/src/seating/seating.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,34 @@
             + self.after
         )
         for expression in self.expressions + self.comments:
             body.insert(expression[1], expression[0])
         return body
 
 
+def fix_type_ignore(source: str) -> str:
+    """Fix misplacement of `# type: ignore` comments in sorted `source`.
+
+    Corrects when
+    >>> var = 6 # type: ignore
+
+    gets turned into
+
+    >>> # type: ignore
+    >>> var = 6"""
+    lines = source.splitlines(True)
+    clean = lambda s: s.replace(" ", "").replace("\n", "")
+    for i, line in enumerate(lines):
+        if clean(line) == "#type:ignore" and 0 < i < len(lines):
+            lines[i] = ""
+            if "#type:ignore" not in clean(lines[i + 1]):
+                lines[i + 1] = lines[i + 1].strip("\n") + "# type: ignore\n"
+    return "".join(lines)
+
+
 def seat(
     source: str, start_line: int | None = None, stop_line: int | None = None
 ) -> str:
     """Sort the contents of classes in `source`, where `source` is parsable Python code.
     Anything not inside a class will be untouched.
 
     The modified `source` will be returned.
@@ -168,15 +188,16 @@
                                 order.functions.append(child)
                         else:
                             order.functions.append(child)
                     except Exception as e:
                         print(ast.dump(child, indent=2))
                         raise e
                 tree.body[i].body = order.sort()
-    return ast.unparse(tree)
+    source = ast.unparse(tree)
+    return fix_type_ignore(source)
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument("file", type=str, help=""" The file to format. """)
     parser.add_argument(
```

### Comparing `seating-0.0.1/LICENSE.txt` & `seating-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seating-0.0.1/README.md` & `seating-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `seating-0.0.1/pyproject.toml` & `seating-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 7365 6174 696e 6722 0d0a 6465 7363   "seating"..desc
 00000070: 7269 7074 696f 6e20 3d20 2253 6f72 7420  ription = "Sort 
 00000080: 7468 6520 6f72 6465 7220 6f66 2063 6c61  the order of cla
 00000090: 7373 2066 756e 6374 696f 6e73 2061 6e64  ss functions and
 000000a0: 2070 726f 7065 7274 6965 7322 0d0a 7665   properties"..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e30 2e31 220d  rsion = "0.0.1".
+000000b0: 7273 696f 6e20 3d20 2230 2e30 2e32 220d  rsion = "0.0.2".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6173  endencies = ["as
 000000f0: 745f 636f 6d6d 656e 7473 222c 2022 626c  t_comments", "bl
 00000100: 6163 6b22 2c20 2270 6174 6869 6572 222c  ack", "pathier",
 00000110: 2022 7079 7465 7374 225d 0d0a 7265 6164   "pytest"]..read
 00000120: 6d65 203d 2022 5245 4144 4d45 2e6d 6422  me = "README.md"
```

### Comparing `seating-0.0.1/PKG-INFO` & `seating-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seating
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sort the order of class functions and properties
 Project-URL: Homepage, https://github.com/matt-manes/seating
 Project-URL: Documentation, https://github.com/matt-manes/seating/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/seating/tree/main/src/seating
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: alphabetical,order,sort,style
```

