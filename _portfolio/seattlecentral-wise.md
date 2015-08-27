---
layout: page
title: Seattle Central W.I.S.E.
name: Seattle Central W.I.S.E.
description: Seattle Central WISE is a custom WordPress theme, utilizing HTML and CSS for presentation, and JQuery for mobile navigation. I also used a WordPress plugin for an image gallery.
githubLink: https://github.com/dougdoner/web170
siteLink: http://designbydoug.com/wise-site
skills: HTML, CSS, JavaScript, WordPress
role: Front End Developer
imgClass: wise
order: 2
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