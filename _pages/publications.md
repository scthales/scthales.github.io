---
layout: page
permalink: /publications/
title: publications
description:
years: [In review, 2021, 2020, 2018, 2015, Thesis]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
