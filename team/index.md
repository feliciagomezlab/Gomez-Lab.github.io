---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our lab is more than just a place of work—it’s a vibrant community where innovation thrives, and young scientists are nurtured through hands-on experience. We believe in the power of teamwork and foster a supportive environment where creativity and curiosity drive our pursuit of groundbreaking discoveries.

Our lab brings together scientists committed to advancing bioinformatics, genomics, and precision oncology. Get to know our team below.

{% include section.html %}

<div style="display: flex; flex-direction: column; gap: 60px;">

  {% assign sorted_team = site.members | sort: 'order' %}
  {% for member in sorted_team %}
    <div style="display: flex; flex-direction: row; align-items: flex-start;">
      <div style="width: 250px; height: 270px; overflow: hidden; margin-right: 30px;">
        <img src="{{ site.baseurl }}/images/team/{{ member.image }}" alt="{{ member.title }}" style="width: 250px; height: 270px; object-fit: cover;">
      </div>
      <div>
        <h3><a href="{{ member.url }}">{{ member.title }}</a></h3>
        <p><strong>Role:</strong> {{ member.role }}</p>
        <p>{{ member.content | markdownify }}</p>
        <div style="margin-top: 10px;">
          {% if member.github %}<a href="{{ member.github }}"><i class="fab fa-github"></i></a>{% endif %}
          {% if member.twitter %}<a href="{{ member.twitter }}"><i class="fab fa-twitter"></i></a>{% endif %}
          {% if member.linkedin %}<a href="{{ member.linkedin }}"><i class="fab fa-linkedin"></i></a>{% endif %}
          {% if member.orcid %}<a href="{{ member.orcid }}"><i class="fab fa-orcid"></i></a>{% endif %}
          {% if member.website %}<a href="{{ member.website }}"><i class="fas fa-link"></i></a>{% endif %}
        </div>
      </div>
    </div>
  {% endfor %}

</div>

{% include section.html %}

{% capture content %}
[![NCI](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/nci-logo.png)](https://www.cancer.gov/)
[![WashU](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/Washu_medicine.png)](https://medicine.wustl.edu/)
[![AGRS](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/ACS-1.png)](https://www.americanresearchgrants.org/)
{% endcapture %}

{% include grid.html content=content %}
