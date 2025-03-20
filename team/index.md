---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our lab is more than just a place of work—it’s a vibrant community where innovation thrives, and young scientists are nurtured through hands-on experience. We believe in the power of teamwork and foster a supportive environment where creativity and curiosity drive our pursuit of groundbreaking discoveries.

{% include section.html %}

<!-- List all team members vertically -->
{% assign members = site.members | sort: "role" | reverse %}
{% for member in members %}
  {% if member.role == "pi" %}
    {% assign member.bio = "Felicia Gomez is the Principal Investigator of the Gomez Lab at Washington University in St. Louis, leading research in cancer genomics and integrative genomic analysis." %}
  {% endif %}
  {% include member-card.html member=member %}
{% endfor %}

{% include section.html background="images/stock_image/background.jpg" dark=true %}

{% include section.html %}
## Funding

{% capture content %}
[![NCI](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/nci-logo.png)](https://www.cancer.gov/)

[![WashU](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/Washu_medicine.png)](https://medicine.wustl.edu/)

[![AGRS](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/ACS-1.png)](https://www.americanresearchgrants.org/)
{% endcapture %}

{% include grid.html content=content %}
