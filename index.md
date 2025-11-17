---
layout: default
title: Home
---

# CS Projects

Computer Science Projects created in the pursuit of a Bachelor's Degree in Computer Science at Western Governors University.

<div class="projects-grid">
  {% for project in site.projects %}
  <div class="project-card">
    {% if project.thumbnail %}
      <img src="{{ project.thumbnail }}" alt="{{ project.title }} thumbnail">
    {% endif %}
    <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
    <h3>{% if project.lan %}
         <i>{{ project.lan }}</i>
    {% endif %}</h3>
  </div>
  {% endfor %}
</div>
