---
layout: default
title: Home
---

# WGU Projects

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


test images
<ul>
  {% assign img_files = site.static_files | where_exp: "file", "file.path contains 'assets/img/'" %}
  {% for file in img_files %}
    <li>
      <a href="{{ file.path | relative_url }}">{{ file.name }}</a>
    </li>
  {% endfor %}
</ul>
