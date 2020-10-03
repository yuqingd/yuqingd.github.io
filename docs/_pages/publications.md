---
layout: page
permalink: /publications/
title: 
description:
years: [2020,2019]
nav: true
---

<div class="publications">
<h3> Preprints </h3>

{% bibliography -f preprints %}
</div>

<div class="publications">
<h3> Publications </h3>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
