---
layout: page
permalink: /publications/
title: publications
order: 2
description: 
years: [2022, 2021, 2020, 2019, 2015]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
