---
layout: page
title: Papers
modified: 2014-07-31T13:23:02.362000-04:00
image:
  feature: sample-image-1.jpg
---


## Preprints 

<ul style="list-style:none">
{% for p in site.data.preprints %}

<li class="paper">
{{p.authors}} ({{p.status}}) {{p.title}} <i>{{p.journal}}</i>. 
<i class="fa fa-link"></i> <a href="http://dx.doi.org/{{p.doi}}">{{p.doi}}</a></li>
{% endfor %}
</ul>

## Published

<ul style="list-style:none">
{% for p in site.data.papers %}

<li class="paper">
{{p.authors}} ({{p.year}}) {{p.title}} <i>{{p.journal}}</i>. {{p.issue}}{% if p.pages %}:{{p.pages}}{% endif %}
<i class="fa fa-link"></i> <a href="http://dx.doi.org/{{p.doi}}">{{p.doi}}</a></li>
{% endfor %}
</ul> 
