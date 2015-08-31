---
layout: page
title: Software
modified: 2014-07-31T13:23:02.362000-04:00
image:
  feature: sample-image-1.jpg
---

{% include _toc.html %}

<ul style="list-style:none">
{% for s in site.data.software %}
<li>
    <h2>{{s.name}}</h2>
    {{s.description}}<br>
    <ul class="software">
    <li><i fa-fw fa-2x class="fa fa-github"></i><a href="http://github.com/{{ s.github }}"> Source</a></li>
{% if s.cran %}
    <li><i fa-fw fa-2x class="fa fa-code"></i> <a href="http://cran.rstudio.com/web/packages/{{s.name}}/index.html">CRAN release</a></li>
{% endif  %}
{% if s.doi %}
    <li><i fa-fw fa-2x class="fa fa-book"></i><a href="http://dx.doi.org/{{ s.doi }}"> Paper</a></li>
{% endif  %}
    </ul>
      
</li>
{% endfor %}
</ul>

