---
layout: default
title: Home
---

## Hi, I'm Jeremy!

I’m a data engineer who built this site as a place to create, learn, and share my thoughts on data, career growth, and whatever else comes to mind.

I'm originally from Southern California. Before moving into data, I spent a decade in Nashville pursuing music. I first got interested in data and analytics while marketing my own drum school, which sparked a new direction for my career.

During the COVID pandemic, I made the transition into data analytics. My work quickly expanded into data engineering, where I discovered I enjoyed building reliable data pipelines, designing data models, and developing the infrastructure that makes data useful.

That path led me to an opportunity at a startup, where I helped build its data infrastructure from the ground up. Today, I work in the utility industry and continue to grow my expertise in data engineering and analytics engineering.

Outside of data, I'm a husband to an amazing wife, a dad of two, and a proud owner of an Aussiedoodle.

___

<h2 id="projects">Projects</h2>

<div class="projects-grid">
  {% for project in site.data.projects %}
    {% include project-card.html project=project %}
  {% endfor %}
</div>

___

<h2 id="blog">Latest Blog Posts</h2>

<div class="projects-grid">
  {% assign latest_posts = site.posts | slice: 0, 4 %}

  {% for post in latest_posts %}
    {% include blog-card.html post=post %}
  {% endfor %}
</div>
