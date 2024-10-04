---
title: Research
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

Explore our extensive range of publications to gain deeper insights into our work. 

{% include section.html %}

## Highlighted

{% include citation.html lookup="Open collaborative writing with Manubot" style="rich" %}

{% include section.html %}

## All

{% include search-box.html %}

{% include search-info.html %}

{% assign papers = site.data.citations | where_exp: "item", "item.type == 'journal-article' or item.type == 'conference-paper'" %}
{% for citation in papers %}
  {% include list.html data="citations" component="citation" %}
{% endfor %}
