---
layout: page
title: Projects
subTitle: Douglas Doner
order: 1
---

{% for project in site.data.projects %}
  {% if project.name %}
  <h2>{{project.name}}</h2>
  <p>{{project.description}}</p>
  <a class="page-link" href="{{ project.githubLink | prepend: site.baseurl }}">GitHub Link</a>
  	{% if project.siteLink %}
  	<a href="{{ project.siteLink}}" target="_blank">Live site</a>
  	{% endif %}
  {% endif %}
{% endfor %}