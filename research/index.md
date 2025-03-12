---
title: Research
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %} Research

Explore our extensive range of publications to gain deeper insights into our work. 

{% include section.html %}

## Selected Publications

<div style="display: flex; gap: 15px; flex-wrap: wrap; margin-bottom: 20px;">
  {% assign years = "2024,2023,2022,2021,2020,2019,2018,2017,2016,Older,All" | split: "," %}
  {% for year in years %}
    <a href="#{{ year | downcase }}" style="text-decoration: none; color: #666; font-size: 18px;">{{ year }}</a>
  {% endfor %}
</div>

{% assign grouped_papers = site.data.citations | group_by_exp: "item", "item.date | slice: 0, 4" | sort: "name" | reverse %}

{% for group in grouped_papers %}
## <a id="{{ group.name | downcase }}"></a> {{ group.name }}

{% for item in group.items %}
<div style="background: #f8f9fa; padding: 20px; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1); margin-bottom: 24px; display: flex; justify-content: space-between; align-items: center;">
  
  <div style="flex: 1;">
    <h3 style="margin-top: 0; font-size: 20px;"><a href="{{ item.link }}" style="text-decoration: none; color: #0056b3;">{{ item.title }}</a></h3>
    <p><strong>Authors:</strong> {{ item.authors | join: ", " }}</p>
    <p><strong>Published in:</strong> {{ item.publisher }} ({{ item.date }})</p>
    <p><strong>DOI:</strong> <a href="{{ item.link }}" style="color: #007bff;">{{ item.id }}</a></p>
  </div>

  <div style="margin-left: 20px;">
    <div data-badge-popover="right" data-badge-type="donut" data-doi="{{ item.id | remove: 'doi:' }}" class="altmetric-embed"></div>
  </div>
</div>
{% endfor %}
{% endfor %}

<script async src="https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js"></script>
