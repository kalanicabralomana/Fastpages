---
keywords: fastai
description: Truth Table
title: Algorithms and Logic
toc: true
comments: true
categories: [code]
nb_path: _notebooks/2022-12-1-truth-table.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-12-1-truth-table.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Truth table = has a designated column for each input variable and one column showing the possible results of the logical operation (and, or, xor, not)</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-javascript"><pre><span></span><span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;AND: 7 &amp; 4&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Thinking: 111 &amp; 100 --&gt; 100&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Answer: 4&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Test:&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="mf">7</span> <span class="o">&amp;</span> <span class="mf">4</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">()</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;OR: 5 | 3&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Thinking: 101 | 011 --&gt; 111&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Answer: 7&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Test:&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="mf">5</span> <span class="o">|</span> <span class="mf">3</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">()</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;XOR: 2 ^ 8&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Thinking: 0010 ^ 1000 --&gt; 1010&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Answer: 10&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Test:&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="mf">9</span> <span class="o">^</span> <span class="mf">3</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">()</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;NOT: ! 1&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Thinking: false is 1 in binary, not true is false&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Answer: true&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="s2">&quot;Test:&quot;</span><span class="p">)</span>
<span class="nx">console</span><span class="p">.</span><span class="nx">log</span><span class="p">(</span><span class="o">!</span> <span class="mf">1</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>AND: 7 &amp; 4
Thinking: 111 &amp; 100 --&gt; 100
Should print 4
Test:
4

OR: 5 | 3
Thinking: 101 | 011 --&gt; 111
Should print 7
Test:
7

XOR: 2 ^ 8
Thinking: 0010 ^ 1000 --&gt; 1010
Should print 10
Test:
10

NOT: ! 0
Thinking: false is 0 in binary, so ! 1011 is not false which is true
Should print true
Test:
false
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

