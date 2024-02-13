---
layout: page
permalink: /publications/
title: Publications
description: List of my publications in reversed chronological order.
years: [2024, 2023, 2022]
nav: true
nav_order: 1
---
For the complete list of publications, you can check my [Google Scholar](https://scholar.google.com/citations?user=6sdzR98AAAAJ&hl=en&oi=ao) profile.

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
