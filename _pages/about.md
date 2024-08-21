---
layout: about
title: about
permalink: /
subtitle: <span style='font-size:1.0em;'>Graduate Research Fellow| Department of Electrical Engineering| University of Texas at San Antonio</span>

profile:
  align: right
  image: pkr.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p style="font-size:0.68em;">Unmanned Systems Laboratory</p>
    <p style="font-size:0.68em;">The University of Texas at San Antonio</p>
    <p style="font-size:0.68em;">San Antonio, Texas 78249</p>

news: false # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

<p>I am currently pursuing my Ph.D. degree in electrical engineering at the University of Texas at San Antonio.</p>
<p>Prior to this, I worked as a project engineer at the VTOL and helicopter laboratory at the Indian Institute of Technology, Kanpur (IITK). He received his B. Tech and M. Tech degrees in Aerospace Engineering from IITK in 2019.</p> 
<p>My research interests include autonomous guidance and control, motion-planning of multi-agent systems, system identification, and flight dynamics modeling.</p>

---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 2
display_categories: [Relational Maneuvering Guidance and Control]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="grid">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}
