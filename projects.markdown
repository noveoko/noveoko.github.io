---
layout: page
title: Projects
permalink: /projects/
---

# My Projects

Browse through a selection of my recent work. Each project represents a unique challenge and solution.

<div class="projects-grid">
  {% for project in site.projects %}
  <div class="project-card">
    <a href="{{ project.url | relative_url }}">
      <div class="project-image">
        <img src="{{ project.thumbnail | relative_url }}" alt="{{ project.title }}">
      </div>
      <div class="project-details">
        <h3>{{ project.title }}</h3>
        <p>{{ project.excerpt }}</p>
        <span class="view-project">View Project</span>
      </div>
    </a>
  </div>
  {% endfor %}
</div>
