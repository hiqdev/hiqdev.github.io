---
layout: page
title: Projects
---

{% for project in site.projects %}
  <h2><a href="/{{ project.title | downcase }}">{{ project.title }}</a></h2>
  {{ project.description }}<br>
  <a href="/{{ project.title || downcase }}/docs">docs</a> &middot;
  <a href="https://github.com/hiqdev/{{ project.title | downcase }}">github</a> &middot;
  <a href="/packages">{{ project.packages_num }} packages</a>

{% endfor %}
