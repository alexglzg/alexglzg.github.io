---
layout: page
title: projects
permalink: /projects/
description: Projects.
nav: true
nav_order: 1
display_categories: [research]
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
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

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
{% endif %}
</div>


<!-- Robust Control of ASVs (where I will talk about all my work on sliding mode for vessels, a lot of papers fit here)
Fast motion planning in highly structured environments (ICRA 2026, PhD work)
Collision avoidance for ASVs (work in Mexico using MPC with buoys, 2-3 papers)
Deep RL for ASVs (ICRA 2023 paper + 2 papers in mexico with ADP)
ASV-UAV Heterogeneous Teams (ICUAS paper, work for the RoboBoat competiton)
Robust Control of UUVs (sliding mode for UUVs, 2 papers)
Safe Planning and Control of ASVs (MPC-CBF frameworks, ICRA 2024+IROS 2025)
Data Enabled Learning (2026 CEP paper on gain tuning via optimization)
Interaction-Aware Motion Planning (MPPI work on multiple vessels, adding link to project at TU Delft https://autonomousrobots.nl/paper_websites/ia-mppi)
Self-Reconfigurable Robotic Boats (work on multiple vessels assembling into structures)
Safe Distributed Motion Planning (ADMM-CBF work on maglevs, accepted for ECC 2026) -->