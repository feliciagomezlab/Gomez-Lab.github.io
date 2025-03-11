---
title: Research
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

Explore our extensive range of publications to gain deeper insights into our work.

{% include section.html %}

## All

{% include search-box.html %}

{% include search-info.html %}

{% include list.html data="citations" component="citation" style="rich" %}

## Altmetric Badges
{% for citation in site.data.citations %}
- {{ citation.title }}
  <div class='altmetric-embed' data-doi='{{ citation.id }}'></div>
{% endfor %}
