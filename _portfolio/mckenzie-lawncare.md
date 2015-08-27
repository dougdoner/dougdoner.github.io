---
layout: page
title: Mckenzie Lawncare
name: Mckenzie Lawncare
description: Mckenzie Lawncare is a static HTML website, using CSS media queries and JQuery to create a mobile responsive experience. I used JQuery for the mobile navigation, as well as PHP includes for repetitive content such as the header and footer.
siteLink: http://designbydoug.com/web200/protosite
skills: HTML, CSS, JavaScript, PHP
role: Front End Developer
imgClass: lawncare
order: 3
---

<div class="columns-9">
  <div class="work-container">
  {% if page.name %}
    <h3>Role: {{ page.role }}</h3>
    <p>{{ page.description }}</p>
    <ul>
    {% if page.siteLink %}
      <li><a href="{{ page.siteLink }}" target="_blank">Live site</a>
    {% endif %}
    {% if page.githubLink %}
      <li><a href="{{ page.githubLink | prepend: site.baseurl }}" target="_blank">GitHub Link</a>
    {% endif %}  
    </ul>
    
  {% endif %}
  </div>
</div>