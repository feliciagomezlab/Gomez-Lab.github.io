---
---
<style>
  header img[src*="logo"] {
    height: 500px !important;
  }
</style>

The Gomez Lab is an interdisciplinary team of scientists who develop and apply computational methods to high-throughput genomic data. We do this work to understand the etiology of cancer and to improve and personalize cancer care.  
We are further driven to increase the application of genomic tools and technologies to populations that are underserved and underrepresented in cancer genomics. Equity in cancer research and care is the framework that drives our research. 


{% include section.html %}

<h2>Highlights</h2>

{% capture text %}

Currently, our research is focused on the genomics of hematological cancers.  Check out our work related to Hodgkin lymphoma and multiple myeloma.

{%
  include button.html
  link="team"
  text="Meet Our Team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/stock_image/CancerAi.jpg"
  link="research"
  title="Our Research"
  text=text
%}
