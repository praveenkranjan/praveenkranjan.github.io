---
layout: about
title: about
permalink: /
subtitle: <span style='font-size:1.0em;'>Graduate Research Fellow| Department of Electrical Engineering</span>

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
social: true # includes social icons at the bottom of the page
---

<p>Pursuing a Ph.D. in Electrical Engineering (Systems & Controls) at the University of Texas at San Antonio, I focus my research on motion planning for the cooperative and adversarial maneuvering of unmanned aerial vehicles (UAVs). My work primarily involves developing advanced guidance laws that enable UAVs to achieve specific behaviors such as formation flying, enclosing, and swarming, whether in coordination with other UAVs or in response to uncooperative agents. A key feature of my research is the integration of flexibility, safety, and robustness into motion planning algorithms, ensuring that these systems can operate reliably with limited information or reduced communication between agents while maintaining strong mathematical guarantees. </p>
<p>Before embarking on my Ph.D., I served as a project engineer at the VTOL and Helicopter Laboratory, where I developed a Hardware-in-the-Loop (HITL) simulation framework for helicopter UAVs. My academic background includes both a Bachelor's and a Master's degree in Aerospace Engineering from the prestigious Indian Institute of Technology, Kanpur.  </p> 
<p>My research interests encompass a broad range of topics within the field of autonomous systems and robotics, particularly in the areas of autonomous guidance and control, motion planning for multi-agent systems, Deep Learning, vehicle design, system identification, and flight dynamics modeling.</p>
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

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

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
{% endif %}
</div>
