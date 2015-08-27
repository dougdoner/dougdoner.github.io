---
layout: page
title: Portfolio
subTitle: Douglas Doner
order: 2
---

<div class="columns-9">
{% assign portfolio = site.portfolio | sort:"order"  %}
{% for project in portfolio %}
  <div class="work-container">
	{% if project.name %}
	  <h2>{{project.name}}</h2>
	  <h3>Role: {{project.role}}</h3>
	  <p>{{project.description}}</p>
	  {% if project.siteLink %}
	  	<a href="{{ project.siteLink}}" target="_blank">Live site</a>
	  {% endif %}
	  {% if project.githubLink %}
	  <a class="page-link" href="{{ project.githubLink | prepend: site.baseurl }}" target="_blank">GitHub Link</a>
	  {% endif %}
	{% endif %}
  </div>
{% endfor %}
</div>