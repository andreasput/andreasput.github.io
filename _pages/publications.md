---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order. 
years: [2013, 2014, 2015, 2016,2017,2020,2021]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
