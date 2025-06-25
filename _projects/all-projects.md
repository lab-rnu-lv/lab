---
layout: page
title: all-projects
---

<ul>
  {% assign sorted_projects = site.projects | sort: "order" %}
  {% for project in sorted_projects %}
    <li>
      <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
    </li>
  {% endfor %}
</ul>
