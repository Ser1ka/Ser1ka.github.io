---
layout: page
title: Projects
permalink: /projects/
description: A showcase of my research and engineering work.
nav: true
nav_order: 3
# display_categories: [work, fun]  horizontal: false
---

<div class="projects">
{% assign sorted_projects = site.projects | sort: "importance" %}

<div class="container">
  <div class="row row-cols-1 row-cols-md-2 justify-content-center">
  {% for project in sorted_projects %}
    {% include projects.liquid %}
  {% endfor %}
  </div>
</div>
</div>