---
layout: page
title: PROJECTS
exclude_from_projects: true
---

# 🛠️ ROBOTICS projects
Here you can explore ROBOTICS students projects.<br>
The best projects will participate in the exhibition "IoT Projects Exhibition" (DECEMBER 2025).<br>
To participate, please write (fill the topic "IoT Projects 2025")

## 📨 E-MAIL  <!-- e-mail -->

  <div class="card">
     <img src="https://lab-rnu-lv.github.io/lab/assets/images/email.jpg" alt="Email address" width="240">
  </div>

---

{% assign sorted_projects = site.projects | where_exp: "item", "item.exclude_from_projects != true" | sort: "order" %}
{% for project in sorted_projects %}
  <li>
    <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
  </li>
{% endfor %}
