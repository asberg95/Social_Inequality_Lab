---
layout: page
title: Research
permalink: /research/
description: Active research projects at the Social Inequality Lab.
nav: true
nav_order: 3
horizontal: True
---
<!-- pages/research.md -->
<div class="projects">
{% assign sorted_projects = site.projects | sort: "importance" %}
{% if page.horizontal %}
<div class="container">
  <div class="row row-cols-1 row-cols-md-2">
  {% for project in sorted_projects %}
    {% include projects_horizontal.liquid %}
  {% endfor %}
  </div>
</div>
{% else %}
<div class="row row-cols-1 row-cols-md-3">
  {% for project in sorted_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>
{% endif %}
</div>
