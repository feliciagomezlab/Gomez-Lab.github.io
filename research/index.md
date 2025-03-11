---
title: Research
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

Explore our extensive range of publications to gain deeper insights into our work.

{% include section.html %}

<script async src="https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js"></script>

## All

{% include search-box.html %}

{% include search-info.html %}

{% for citation in citations %}
  <div>
    <h3><a href="{{ citation.link }}">{{ citation.title }}</a></h3>
    <p>{{ citation.authors | join: ", " }}</p>
    <div class="altmetric-embed" data-badge-type="donut" data-doi="{{ citation.id }}"></div>
  </div>
{% endfor %}
