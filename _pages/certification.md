---
layout: page
title: Certification
permalink: /certification/
description: Sharing the certifications I did.
nav: true
nav_order: 4
display_categories: [Machine Learning and AI]
horizontal: false
---

<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_research = site.research | where: "category", category %}
  {% assign sorted_research = categorized_research | sort: "importance" %}
  <!-- Generate cards for each research project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for research in sorted_research %}
      {% include research.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for research in sorted_research %}
      {% include research.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}
{% else %}
{% assign sorted_research = site.research | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for research in sorted_research %}
      {% include research.liquid %}
    {% endfor %}
  </div>
{% endif %}
</div>
