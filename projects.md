---
layout: default
title: Projects
description: A curated list of my GitHub and personal projects
permalink: /projects/
---

# 🚀 My Projects

<div class="project-grid">
  {% for project in site.data.projects %}
    <div class="project-card">
      <h3>{{ project.name }}</h3>
      <p>{{ project.description }}</p>

      <div class="project-links">
        {% if project.github %}
          <a href="{{ project.github }}" target="_blank">🔗 GitHub</a>
        {% endif %}
        {% if project.page %}
          <a href="{{ project.page }}">📄 Details</a>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>
