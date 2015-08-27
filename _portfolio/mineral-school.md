---
layout: page
title: Mineral School
name: Mineral School
githubLink: https://github.com/theplanetmike/mineralschool
description: I created a custom WordPress theme from visual design mockups. I created and customized Grunt build scripts for LESS style compilation. I used media queries and JQuery for a mobile responsive design. Agile methedologies were used to organize the timely execution of project goals.
siteLink: http://mineral-school.org
skills: HTML, CSS, JavaScript, WordPress
role: Front End Developer
imgClass: mineral-school
order: 1
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