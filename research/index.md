---
title: Research
nav:
  order: 1
  tooltip: Published works
search: true
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

Explore our extensive range of publications to gain deeper insights into our work. 

{% include section.html %}

## All Publications by Year

<!-- Search Box -->
<div style="margin-bottom: 20px;">
  <input type="text" id="search-box" placeholder="Search publications..." 
         style="width: 100%; padding: 10px; font-size: 16px; border: 1px solid #ccc; border-radius: 5px;">
</div>

<!-- Start of Publication List -->
<div id="publications-list">
  {% assign grouped_papers = site.data.citations | group_by_exp: "item", "item.date | slice: 0, 4" | sort: "name" | reverse %}

  {% for group in grouped_papers %}
  <h2 class="year-header">{{ group.name }}</h2>

  {% for item in group.items %}
  <div class="searchable-item" style="background: #f8f9fa; padding: 20px; border-radius: 10px; box-shadow: 0px 4px 8px rgba(0,0,0,0.1); margin-bottom: 24px; display: flex; justify-content: space-between; align-items: center;">
    <div style="flex: 1;">
      <h3 style="margin-top: 0; font-size: 20px;">
        <a href="{{ item.link }}" style="text-decoration: none; color: #0056b3;">{{ item.title }}</a>
      </h3>
      <p><strong>Authors:</strong> {{ item.authors | join: ", " }}</p>
      <p><strong>Published in:</strong> {{ item.publisher }} ({{ item.date }})</p>
      <p><strong>DOI:</strong> <a href="{{ item.link }}" style="color: #007bff;">{{ item.id }}</
