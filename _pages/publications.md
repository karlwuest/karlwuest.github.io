---
layout: page
permalink: /publications/
title: publications
years: [2021, 2020, 2019, 2018, 2017, 2016]
nav: true
---

<div class="publications">

<h1>peer-reviewed</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1>tech reports</h1>
  {% bibliography -f techreports %}
</div>


