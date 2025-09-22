---
title: Research
nav:
  order: 1
  tooltip: Published works
---

<h1>Research</h1>

{% include section.html %}

<h2>Selected Publications</h2>

{% assign grouped_papers = site.data.citations | group_by_exp: "item", "item.date | slice: 0, 4" | sort: "name" | reverse %}

{% for group in grouped_papers %}

<h2>{{ group.name }}</h2>

{% for item in group.items %}
  {% unless item.id == "doi:10.1101/266262" or item.id == "doi:10.1101/2021.06.25.21258374" %}
  <div style="background: #f8f9fa; padding: 20px; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1); margin-bottom: 24px;">

    <!-- Title + Badge side by side -->
    <div style="display: flex; align-items: center; justify-content: space-between;">
      <h3 style="margin: 0; font-size: 20px; flex: 1;">
        <a href="{{ item.link }}" style="text-decoration: none; color: #0056b3;">
          {{ item.title }}
        </a>
      </h3>
      <!-- Altmetric badge -->
      <div class="altmetric-embed" 
           data-badge-type="donut" 
           data-badge-popover="right" 
           data-doi="{{ item.id | remove: 'doi:' }}">
      </div>
    </div>

    <!-- Authors -->
    <p style="margin-top: 10px;"><strong>Authors:</strong> {{ item.authors | join: ", " }}</p>

    <!-- Journal info -->
    <p><strong>Published in:</strong> {{ item.publisher }} ({{ item.date }})</p>

    <!-- DOI -->
    <p><strong>DOI:</strong> <a href="{{ item.link }}" style="color: #007bff;">{{ item.id }}</a></p>

  </div>
  {% endunless %}
{% endfor %}
{% endfor %}

<!-- Load Altmetric script once -->
<script async src="https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js"></script>
