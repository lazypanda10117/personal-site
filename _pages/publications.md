---
layout: page
title: Publications
permalink: /publications/
description: in reverse chronological order
years: [2020,2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
