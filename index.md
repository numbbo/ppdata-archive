---
layout: default
permalink: /
nav_exclude: true
title: Home
---
# COCO postprocessed data archive  #
---

COCO (COmparing Continuous Optimizers) is a platform for systematic and sound comparisons of real-parameter global optimizers. Here, we provide postprocessed data from all 300+ officially supported algorithm data sets for the various available test suites. Due to the large amount of algorithms (and the limited space in the figures), we group algorithm data sets by year of publication.


<table>
<tr>
  <th><h2>bbob</h2></th>
  <th><h2>bbob-noisy</h2></th>
  <th><h2>bbob-biobj</h2></th>
  <th><h2>bbob-largescale</h2></th>
  <th><h2>bbob-mixint</h2></th>
  <th><h2>bbob-constrained</h2></th>
</tr>
<tr>
  <td>24 functions<br />
	  single-objective<br />
	  continous domain<br />
	  200+ algorithm data sets
  </td>
  <td>30 functions<br />
	  noisy evaluations<br />
	  single-objective<br />
	  45 algorithm data sets
  </td>
  <td>55 functions<br />
	  bi-objective<br />
	  noiseless<br />
	  30+ algorithm data sets
  </td>
  <td>24 bbob functions<br />
	  single-objective<br />
	  dimensions 20 to 640<br />
	  11 algorithm data sets   
  </td>
  <td>24 functions<br />
	  80&#37; discrete variables<br />
	  single-objective<br />
	  4 algorithm data sets
  </td>
  <td>54 functions<br />
      from 9 &quot;raw&quot; bbob functions with<br />
      1 to (9 + &lfloor; 9n/2 &rfloor;) non-linear constraints<br />
	  1 baseline algorithm data set
  </td>
</tr>
<tr>
  <td style="text-align:center">
    <a href="./bbob/2009/index.html">2009</a><br />
	<a href="./bbob/2010/index.html">2010</a><br />
	<a href="./bbob/2012/index.html">2012</a><br />
	<a href="./bbob/2013/index.html">2013</a><br />
	<a href="./bbob/2014/index.html">2014</a><br />
	<a href="./bbob/2015-CEC/index.html">2015-CEC</a><br />
	<a href="./bbob/2015-GECCO/index.html">2015-GECCO</a><br />
	<a href="./bbob/2016/index.html">2016</a><br />
	<a href="./bbob/2017/index.html">2017</a><br />
	<a href="./bbob/2018/index.html">2018</a><br />
	<a href="./bbob/2019/index.html">2019</a><br />
  </td>
  <td style="text-align:center">
    <a href="./bbob-noisy/2009/index.html">2009</a><br />
    <a href="./bbob-noisy/2010/index.html">2010</a><br />
	<a href="./bbob-noisy/2012/index.html">2012</a><br />
	<a href="./bbob-noisy/2016/index.html">2016</a><br />
  </td>   
  <td style="text-align:center">
    <a href="./bbob-biobj/2016/index.html">2016</a><br />
	<a href="./bbob-biobj/2017/index.html">2017</a><br />
	<a href="./bbob-biobj/2019/index.html">2019</a><br />
  </td>  
  <td style="text-align:center">
	<a href="./bbob-largescale/2019/index.html">2019</a>
  </td>  
  <td style="text-align:center">
    <!--<a href="./bbob-mixint/2019/index.html">2019</a>-->
  </td>
  <td style="text-align:center">
    <!--<a href="./bbob-constrained/2022/index.html">2022</a>-->
  </td>
</tr>
</table>

The Python code to locally generate the first entry, bbob 2009,
in the table (other entries work respectively) reads

<pre>
<code class="python">
import cocopp               # see https://pypi.org/project/cocopp
cocopp.main('bbob/2009/*')  # will take several minutes to process
</code>
</pre>


Related links
---------------

* [raw data listing](https://numbbo.github.io/data-archive)
* [how to submit a data set](https://github.com/numbbo/coco/blob/master/howtos/publish-a-dataset-howto.md)
* [how to create and use COCO data archives with the cocopp.archiving Python module](https://github.com/numbbo/coco/blob/master/code-postprocessing/cocopp/archiving.py)







Citation
--------

You may cite this work in a scientific context as

N. Hansen, A. Auger, R. Ros, O. Mersmann, T. Tušar, D. Brockhoff. [COCO: A Platform for Comparing Continuous Optimizers in a Black-Box Setting](https://doi.org/10.1080/10556788.2020.1808977), _Optimization Methods and Software_, 36(1), pp. 114-144, 2021. [[pdf](https://www.tandfonline.com/eprint/DQPF7YXFJVMTQBH8NKR8/pdf?target=10.1080/10556788.2020.1808977), [arXiv](https://arxiv.org/abs/1603.08785)]

{% raw %}
```latex
    @ARTICLE{hansen2021coco,
    author = {Hansen, N. and Auger, A. and Ros, R. and Mersmann, O. and Tu{\v s}ar, T. and Brockhoff, D.},
    title = {{COCO}: A Platform for Comparing Continuous Optimizers in a Black-Box Setting},
    journal = {Optimization Methods and Software},
    doi = {https://doi.org/10.1080/10556788.2020.1808977},
    pages = {114--144},
    issue = {1},
    volume = {36},
    year = 2021
    }
```
{% endraw %}

<link rel="stylesheet" href="{{ '/assets/css/custom.css' | relative_url }}"/>
