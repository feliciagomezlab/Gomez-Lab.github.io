---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

<h1>Contact</h1>

{%
  include button.html
  type="email"
  text="fgomez@wustl.edu"
  link="fgomez@wustl.edu"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://www.google.com/maps/place/Mid+Campus+Center/@38.6362236,-90.2619309,15z/data=!4m6!3m5!1s0x87d8b4df564ad7d1:0xddebd7786d830554!8m2!3d38.6362236!4d-90.2619309!16s%2Fg%2F11dxqfct18?entry=ttu"
%}

{% include section.html %}

<div style="text-align: center;">
  {% include figure.html image="images/location/MCC.jpg" caption="" %}
</div>

{% include section.html dark=true %}

{% capture col1 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col2 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col3 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
