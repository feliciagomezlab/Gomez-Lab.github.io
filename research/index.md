---
title: Research
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

Explore our extensive range of publications to gain deeper insights into our work. 

{% include section.html %}

## All Publications by Year

{% include search-box.html %}

{% include search-info.html %}

{% assign grouped_papers = site.data.citations | group_by_exp: "item", "item.date | slice: 0, 4" | sort: "name" | reverse %}

{% for group in grouped_papers %}
## {{ group.name }}

{% for item in group.items %}
<div style="display: flex; justify-content: space-between; align-items: center; width: 100%; background: #f8f9fa; padding: 20px; border-radius: 10px; box-shadow: 0px 2px 10px rgba(0,0,0,0.1); margin-bottom: 20px;">
  <div style="flex: 1;">
    <h3 style="margin-top: 0;">{{ item.title }}</h3>
    <p><strong>Authors:</strong> {{ item.authors | join: ", " }}</p>
    <p><strong>Published in:</strong> {{ item.publisher }} ({{ item.date }})</p>
    <p><strong>DOI:</strong> <a href="{{ item.link }}">{{ item.id }}</a></p>
  </div>
  <div style="margin-left: 20px;">
    <div data-badge-popover="right" data-badge-type="donut" data-doi="{{ item.id | remove: 'doi:' }}" class="altmetric-embed"></div>
  </div>
</div>
{% endfor %}
{% endfor %}

<script async src="https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js"></script>
