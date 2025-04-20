---
layout: page
title: Certification
permalink: /certification/
description: Sharing the certifications I did.
nav: true
nav_order: 4
display_categories: [ML]
horizontal: false
---

<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_certification = site.certification | where: "category", category %}
  {% assign sorted_certification = categorized_certification | sort: "importance" %}
  <!-- Generate cards for each certification project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for certification in sorted_certification %}
      {% include certification.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for certification in sorted_certification %}
      {% include certification.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}
{% else %}
{% assign sorted_certification = site.certification | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for certification in sorted_certification %}
      {% include certification.liquid %}
    {% endfor %}
  </div>
{% endif %}
</div>
