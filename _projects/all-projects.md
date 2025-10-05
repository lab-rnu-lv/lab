---
layout: page
title: PROJECTS
exclude_from_projects: true
---

# 🛠️ ROBOTICS projects
Here you can explore ROBOTICS students projects.
The best projects will participate in the exhibition "IoT Projects Exhibition" (DECEMBER 2025).

---

{% assign sorted_projects = site.projects | where_exp: "item", "item.exclude_from_projects != true" | sort: "order" %}
{% for project in sorted_projects %}
  <li>
    <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
  </li>
{% endfor %}
