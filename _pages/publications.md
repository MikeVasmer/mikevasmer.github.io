---
layout: page
permalink: /publications/
title: Publications
description: 
yearsPub: [2026, 2025, 2024, 2023, 2022, 2021, 2019]
yearsPre: [2026, 2025, 2024]
yearsThe: [2019]
nav: true
nav_order: 1
---

<!-- For an up to date list, see my <a href=https://scholar.google.com/citations?hl=en&user=YWXgW2wAAAAJ&view_op=list_works>Google Scholar page</a>. -->
<!-- _pages/publications.md -->

For an up-to-date list, see my [Google Scholar page](https://scholar.google.com/citations?hl=en&user=YWXgW2wAAAAJ&view_op=list_works).

## Published articles

<div class="publications">
{%- for y in page.yearsPub %}
  <!-- <h2 class="year">{{y}}</h2> -->
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

## Preprints

<div class="publications">
{%- for y in page.yearsPre %}
  <!-- <h2 class="year">{{y}}</h2> -->
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}
</div>

## PhD thesis

<div class="publications">
{%- for y in page.yearsThe %}
  <!-- <h2 class="year">{{y}}</h2> -->
  {% bibliography -f theses -q @*[year={{y}}]* %}
{% endfor %}
</div>
