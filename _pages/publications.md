---
layout: page
permalink: /publications/
title: publications
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
---

<div class="publications">
<h4>Please visit the <a href="https://scholar.google.com/citations?user=dMK8VBkAAAAJ&hl=en">Google Scholar Page</a> for full publications.</h4>
{% for y in page.years %}
  <h2 class="year"><strong>{{y}}</strong></h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
