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
  <div style="display: flex; flex-direction: row; align-items: center;">
    <div style="width: 220px; height: 220px; overflow: hidden; margin-right: 30px;">
      <img src="{{ site.baseurl }}/images/team/Batchi_Armel.jpg" alt="Armel Batchi-Bouyou" style="width: 100%; height: 100%; object-fit: cover;">
    </div>
    <div>
      <h3>Armel Batchi-Bouyou</h3>
      <p>Postdoctoral Research Associate</p>
      <p>Armel is a postdoctoral research associate in the Gomez Lab, focusing on cancer genomics and molecular mechanisms of cancer. He plays a key role in developing new analytical approaches for cancer data and integrating multi-omics datasets to drive discovery in oncology research.</p>
      <div>
        <a href="https://www.linkedin.com/in/armel-batchi-bouyou/" target="_blank" title="LinkedIn">
          <i class="fa-brands fa-linkedin" style="font-size: 20px; margin-right: 10px;"></i>
        </a>
        <a href="https://scholar.google.com/citations?user=YOUR_GOOGLE_SCHOLAR_ID" target="_blank" title="Google Scholar">
          <i class="fa-brands fa-google" style="font-size: 20px;"></i>
        </a>
      </div>
    </div>
  </div>
  <hr style="border: 1px solid #ccc; width: 100%; margin-top: 20px; margin-bottom: 20px;">

  <div style="display: flex; flex-direction: row; align-items: center;">
    <div style="width: 220px; height: 220px; overflow: hidden; margin-right: 30px;">
      <img src="{{ site.baseurl }}/images/team/Charlz.jpeg" alt="Charlz Nithin Jerold" style="width: 200px; height: 200px; object-fit: cover;">
    </div>
    <div>
      <h3>Charlz Nithin Jerold</h3>
      <p>Bioinformatics Research Analyst</p>
      <p>Charlz supports a wide range of bioinformatics analyses, including data preprocessing, somatic variant detection, and statistical interpretation. He brings extensive experience in cancer genomics and software development to the lab.</p>
      <div>
        <a href="https://www.linkedin.com/in/charlz-nithin/" target="_blank" title="LinkedIn">
          <i class="fa-brands fa-linkedin" style="font-size: 20px; margin-right: 10px;"></i>
        </a>
        <a href="https://scholar.google.com/citations?user=qU4svkkAAAAJ" target="_blank" title="Google Scholar">
          <i class="fa-brands fa-google" style="font-size: 20px;"></i>
        </a>
      </div>
    </div>
  </div>
  <hr style="border: 1px solid #ccc; width: 100%; margin-top: 20px; margin-bottom: 20px;">

  <div style="display: flex; flex-direction: row; align-items: center;">
    <div style="width: 220px; height: 220px; overflow: hidden; margin-right: 30px;">
      <img src="{{ site.baseurl }}/images/team/MKhanfar_HSG.jpg" alt="Mariam Khanfar" style="width: 100%; height: 100%; object-fit: cover;">
    </div>
    <div>
      <h3>Mariam Khanfar</h3>
      <p>PhD Candidate</p>
      <p>Mariam is a PhD candidate studying Hodgkin lymphoma and the tumor microenvironment. Her work applies genomic and RNA technologies, such as whole-exome sequencing and single-cell genomics, to advance cancer research and improve our understanding of tumor-immune interactions.</p>
      <div>
        <a href="https://www.linkedin.com/in/mariam-khanfar/" target="_blank" title="LinkedIn">
          <i class="fa-brands fa-linkedin" style="font-size: 20px; margin-right: 10px;"></i>
        </a>
        <a href="https://scholar.google.com/citations?user=0000-0002-3650-2665" target="_blank" title="Google Scholar">
          <i class="fa-brands fa-google" style="font-size: 20px;"></i>
        </a>
      </div>
    </div>
  </div>
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
