---
---

Our lab brings together a diverse group of researchers with expertise in clinical, computational, molecular, and mathematical disciplines, all united by a shared interest in understanding the genomic underpinnings of cancer. We focus specifically on Hodgkin and non-Hodgkin lymphomas, as well as multiple myeloma, investigating how acquired genetic mutations influence the clinical manifestations of these diseases and their responses to treatment.

Classic Hodgkin lymphoma (cHL) presents a unique challenge, accounting for 10% of all lymphomas in the Western world and remaining a significant clinical concern. While many patients respond well to standard therapies, a subset faces relapse or resistance. The disease is characterized by the rare malignant B cells known as Hodgkin-Reed-Sternberg (HRS) cells, which constitute only a small fraction of the tumor environment. Despite advancements in next-generation sequencing, detecting somatic mutations in cancers dominated by these rare cell populations remains difficult, largely due to low signal-to-noise ratios and a lack of sophisticated algorithms designed to handle low variant allele frequency (VAF) variants.

Our research seeks to address these challenges through two main avenues of inquiry:

	1.	Can ultra-deep exome-wide sequencing, combined with tailored filtering and analysis techniques, successfully identify somatic mutations in cHL?
	2.	Do these low VAF somatic mutations, identified from HRS cells using our refined analytical strategies, correlate with disease outcomes in cHL?

Our lab’s mission is to conduct research that directly informs and improves clinical practices in oncology. We are recognized for our strengths in genomic profiling, the development of advanced high-throughput laboratory and bioinformatics methods, and our ability to manage and interpret extensive and complex genomic data. Through our extensive network of research and clinical partnerships, we strive to push the boundaries of cancer research, ultimately enhancing patient care and outcomes.

{% include section.html %}

## Highlights

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="research"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="Our Research"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="projects"
  text="Browse our projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="projects"
  title="Our Projects"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="team"
  title="Our Team"
  text=text
%}
