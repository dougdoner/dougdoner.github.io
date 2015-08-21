---
layout: page
title: Portfolio
subTitle: Douglas Doner
order: 1
---

<div class="columns-9">
{% for project in site.data.projects %}
  <div class="work-container">
	  {% if project.name %}
	  <h2>{{project.name}}</h2>
	  <h3>Role: {{project.role}}</h3>
	  <p>{{project.description}}</p>
	  <a class="page-link" href="{{ project.githubLink | prepend: site.baseurl }}">GitHub Link</a>
	  	{% if project.siteLink %}
	  	<a href="{{ project.siteLink}}" target="_blank">Live site</a>
	  	{% endif %}
	  {% endif %}
  </div>
{% endfor %}
</div>