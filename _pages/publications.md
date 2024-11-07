---
layout: page
permalink: /publications/
title: publications
description: For an up to date list, see <a href=https://arxiv.org/a/vasmer_m_1.html>my arXiv page</a>.
yearsPub: [2024, 2023, 2022, 2021, 2019]
yearsPre: [2024]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
### preprints

<div class="publications">
{%- for y in page.yearsPre %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}
</div>

---

### published articles

<div class="publications">
{%- for y in page.yearsPub %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
