---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our lab is more than just a place of work—it’s a vibrant community where innovation thrives, and young scientists are nurtured through hands-on experience. We believe in the power of teamwork and foster a supportive environment where creativity and curiosity drive our pursuit of groundbreaking discoveries.

{% include section.html %}

<!-- Team Member Section with Vertical Alignment -->
<div class="team-member-list">
  <div class="team-member">
    <div class="team-member-image">
      <img src="{{ site.baseurl }}/images/team/FG.jpg" alt="Felicia Gomez">
    </div>
    <div class="team-member-info">
      <h3>Felicia Gomez</h3>
      <p>Principal Investigator</p>
      <p>Felicia Gomez is the Principal Investigator of the Gomez Lab, specializing in cancer genomics and molecular biology.</p>
      <a href="https://profiles.wustl.edu/en/persons/felicia-gomez">More Info</a>
    </div>
  </div>

  <div class="team-member">
    <div class="team-member-image">
      <img src="{{ site.baseurl }}/images/team/Charlz.jpeg" alt="Charlz Nithin Jerold">
    </div>
    <div class="team-member-info">
      <h3>Charlz Nithin Jerold</h3>
      <p>Bioinformatics Research Analyst</p>
      <p>Charlz supports bioinformatics analyses for the lab, including variant detection and statistical interpretation.</p>
      <a href="https://cnithin7.github.io">More Info</a>
    </div>
  </div>

  <div class="team-member">
    <div class="team-member-image">
      <img src="{{ site.baseurl }}/images/team/Armel.jpg" alt="Armel Batchi-Bouyou">
    </div>
    <div class="team-member-info">
      <h3>Armel Batchi-Bouyou</h3>
      <p>Postdoctoral Research Associate</p>
      <p>Armel is a postdoctoral researcher, focusing on the intersection of molecular biology and oncology.</p>
    </div>
  </div>

  <!-- Add other team members similarly -->
</div>

{% include section.html background="images/stock_image/background.jpg" dark=true %}

{% include section.html %}
## Funding

{% capture content %}
[![NCI](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/nci-logo.png)](https://www.cancer.gov/)

[![WashU](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/Washu_medicine.png)](https://medicine.wustl.edu/)

[![AGRS](https://feliciagomezlab.github.io/Gomez-Lab.github.io/images/funding/ACS-1.png)](https://www.americanresearchgrants.org/)
{% endcapture %}

{% include grid.html content=content %}
