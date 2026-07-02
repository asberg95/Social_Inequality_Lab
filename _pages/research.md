---
layout: page
title: Research
permalink: /research/
description: Active research projects at the Social Inequality Lab.
nav: true
nav_order: 3
horizontal: false
---
<!-- pages/research.md -->
<div class="projects">
{% assign sorted_projects = site.projects | sort: "importance" %}
<div class="row row-cols-1">
  {% for project in sorted_projects %}
    {% include projects.liquid %}
  {% endfor %}
</div>
</div>
