---
title: Team
layout: default
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %} Team

Our lab is more than just a place of work—it’s a vibrant community where innovation thrives, and young scientists are nurtured through hands-on experience...

{% include section.html %}

<div class="team-list">
  {% assign members = site.team | sort: "name" %}
  {% for member in members %}
    <div style="display: flex; flex-direction: row; align-items: center; margin-bottom: 40px;">
      <div style="width: 70%; height: 70%; overflow: hidden; margin-right: 30px;">
        <img src="{{ member.image }}" alt="{{ member.name }}" style="width: 250px; height: 270px; object-fit: cover;">
      </div>
      <div>
        <h3><a href="{{ member.url }}">{{ member.name }}</a></h3>
        <p>{{ member.position }}</p>
        <p>{{ member.excerpt }}</p>
        <div>
          {% if member.linkedin %}
            <a href="{{ member.linkedin }}" target="_blank" title="LinkedIn">
              <i class="fa-brands fa-linkedin" style="font-size: 20px; margin-right: 10px;"></i>
            </a>
          {% endif %}
          {% if member.scholar %}
            <a href="{{ member.scholar }}" target="_blank" title="Google Scholar">
              <i class="fa-brands fa-google" style="font-size: 20px;"></i>
            </a>
          {% endif %}
        </div>
      </div>
    </div>
    <hr style="border: 1px solid #ccc; width: 100%; margin-top: 10px; margin-bottom: 10px;">
  {% endfor %}
</div>
