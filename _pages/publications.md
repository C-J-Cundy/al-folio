---
layout: page
permalink: /publications/
title: publications
description: Publications by categories in reversed chronological order.
years: [2019, 2018, 2017, 2016, 2015, 2014]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
