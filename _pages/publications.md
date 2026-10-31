---
layout: page
permalink: /publications/
title: Publications
lang: en
description:
years: [2026, 2025, 2024, 2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<div class="publications">

<p style="font-family: Arial; font-size: 1rem; margin-bottom: 1.5rem; font-weight: bold;">
  For more up-to-date information, please refer to my 
  <a href="https://scholar.google.com/citations?user=osQ5dAkAAAAJ&hl=en" target="_blank" style="text-decoration: underline;">
    Google Scholar
  </a>.
</p>

<h2><span class="font-weight-bold">Papers</span></h2>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
