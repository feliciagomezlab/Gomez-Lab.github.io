---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our lab is more than just a place of work—it’s a vibrant community where innovation thrives, and young scientists are nurtured through hands-on experience. We believe in the power of teamwork and foster a supportive environment where creativity and curiosity drive our pursuit of groundbreaking discoveries.

{% include section.html %}

<div style="display: flex; flex-direction: column; gap: 40px;">
  {% assign sorted_team = site.members | sort: 'order' %}
  {% for member in sorted_team %}
    <div style="display: flex; flex-direction: row; align-items: center;">
      <div style="width: 70%; height: 70%; overflow: hidden; margin-right: 30px;">
        <img src="{{ site.baseurl }}{{ member.image }}" alt="{{ member.title }}" style="width: 250px; height: 270px; object-fit: cover;">
      </div>
      <div>
        <h3><a href="{{ member.url }}">{{ member.title }}</a></h3>
        <p>{{ member.role }}</p>
        <p>{{ member.content | markdownify }}</p>
        <div>
          {% if member.website %}
            <a href="{{ member.website }}" target="_blank" title="Website"><i class="fa-solid fa-globe" style="font-size: 20px; margin-right: 10px;"></i></a>
          {% endif %}
          {% if member.email %}
            <a href="mailto:{{ member.email }}" title="Email"><i class="fa-solid fa-envelope" style="font-size: 20px; margin-right: 10px;"></i></a>
          {% endif %}
          {% if member.linkedin %}
            <a href="{{ member.linkedin }}" target="_blank" title="LinkedIn"><i class="fa-brands fa-linkedin" style="font-size: 20px; margin-right: 10px;"></i></a>
          {% endif %}
          {% if member.scholar %}
            <a href="{{ member.scholar }}" target="_blank" title="Google Scholar"><i class="fa-brands fa-google" style="font-size: 20px;"></i></a>
          {% endif %}
          {% if member.orcid %}
            <a href="{{ member.orcid }}" target="_blank" title="ORCID"><i class="fa-brands fa-orcid" style="font-size: 20px;"></i></a>
          {% endif %}
        </div>
      </div>
    </div>
    <hr style="border: 1px solid #ccc; width: 100%; margin-top: 10px; margin-bottom: 10px;">
  {% endfor %}
</div>

{% include section.html %}

{% capture content %}
[![NCI](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/nci-logo.png)](https://www.cancer.gov/)
[![WashU](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/Washu_medicine.png)](https://medicine.wustl.edu/)
[![AGRS](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/ACS-1.png)](https://www.americanresearchgrants.org/)
{% endcapture %}

{% include grid.html content=content %}
