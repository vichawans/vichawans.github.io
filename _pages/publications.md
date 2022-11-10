---
layout: page
permalink: /publications/
title: Publications
description: Publications by year
years: [2020, 2018, 2016]
nav: true
nav_order: 1
---

An up-to-date list is available on [Google Scholar](https://scholar.google.com/citations?user=NNHRfwwAAAAJ).


<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
