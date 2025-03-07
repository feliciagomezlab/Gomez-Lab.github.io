---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our lab is more than just a place of work—it’s a vibrant community where innovation thrives, and young scientists are nurtured through hands-on experience. We believe in the power of teamwork and foster a supportive environment where creativity and curiosity drive our pursuit of groundbreaking discoveries.

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}

{% include section.html background="images/background.jpg" dark=true %}

{% include section.html %}
## Funding

{% capture content %}
[![National Cancer Institute](/images/nci-logo.jpg](https://www.cancer.gov/)

[![Washington University School of Medicine](/images/Washu_medicine.jpg](https://medicine.wustl.edu/)

[![American Grants Research Society](/images/ACS-1.png)](https://www.americanresearchgrants.org/)
{% endcapture %}


{% include grid.html style="square" content=content %}
