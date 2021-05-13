---
layout: page
permalink: /publications/
title: Papers
description: <i> <b>P</b>ublish <b>T</b>o <b>P</b>erish. </i>
years: [2021]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
