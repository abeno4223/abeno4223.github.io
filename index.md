---
layout: default
title: Home
---

# Welcome

I am Alexandra Beno, a Software Developer with experience in application design and project management. Below, you will find a collection of projects created throughout my career and time as a student.


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


# Minecraft Modpacks

A collection of custom <a href="https://www.minecraft.net/en-us/about-minecraft">Minecraft</a> modpacks created as an employee of <a href="https://feed-the-beast.com/">Feed the Beast</a>, a member of the Phoenix Team, or independently.

<div class="modpacks-grid">
  {% for project in site.modpacks %}
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