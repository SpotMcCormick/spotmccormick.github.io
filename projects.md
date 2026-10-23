---
layout: default
title: Projects
---

<h2>Projects</h2>

<div class="projects-grid">
  {% for project in site.data.projects %}
    {% include project-card.html project=project %}
  {% endfor %}
</div>
