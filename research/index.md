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
  <input type="text" id="search-box" placeholder="Search items on this page..." 
         style="width: 100%; padding: 10px; font-size: 16px; border: 1px solid #ccc; border-radius: 5px;">
</div>

<!-- Start of Publications List -->
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
      <p><strong>DOI:</strong> <a href="{{ item.link }}" style="color: #007bff;">{{ item.id }}</a></p>
    </div>

    <div style="margin-left: 20px;">
      <div data-badge-popover="right" data-badge-type="donut" data-doi="{{ item.id | remove: 'doi:' }}" class="altmetric-embed"></div>
    </div>

  </div>
  {% endfor %}
  {% endfor %}
</div>

<script async src="https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js"></script>

<!-- 🔍 JavaScript for Full-Page Search -->
<script>
document.addEventListener("DOMContentLoaded", function () {
    let searchBox = document.getElementById("search-box");
    let items = document.querySelectorAll(".searchable-item");
    let yearHeaders = document.querySelectorAll(".year-header");

    if (!searchBox || !items.length) {
        console.error("Search box or items not found.");
        return;
    }

    searchBox.addEventListener("input", function () {
        let query = searchBox.value.toLowerCase().trim();
        let hasResults = false;

        items.forEach(item => {
            let textContent = item.innerText.toLowerCase();
            if (textContent.includes(query)) {
                item.style.display = "flex";
                hasResults = true;
            } else {
                item.style.display = "none";
            }
        });

        // Hide year headers if they have no visible publications
        yearHeaders.forEach(header => {
            let nextElements = [];
            let nextSibling = header.nextElementSibling;
            while (nextSibling && nextSibling.classList.contains("searchable-item")) {
                nextElements.push(nextSibling);
                nextSibling = nextSibling.nextElementSibling;
            }
            let visibleItems = nextElements.filter(item => item.style.display === "flex");
            header.style.display = visibleItems.length ? "block" : "none";
        });

        if (!hasResults) {
            console.warn("No matching results found.");
        }
    });
});
</script>
