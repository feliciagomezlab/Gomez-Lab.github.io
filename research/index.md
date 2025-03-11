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

<script type='text/javascript' src='https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js'></script>

{% for citation in site.data.citations %}
  {% if citation.id contains "doi:" %}
    <div class='altmetric-embed' data-badge-type='donut' data-doi='{{ citation.id | remove: "doi:" }}'></div>
  {% endif %}
{% endfor %}
