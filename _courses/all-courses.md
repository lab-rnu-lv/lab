---
layout: page
title: COURSES
exclude_from_course: true
---


# 📚 Available Courses

Welcome to our course list!  
Here you can explore all available topics sorted by category.

---

{% assign sorted_courses = site.courses | where_exp: "item", "item.exclude_from_course != true" | sort: "order" %}

{% for course in sorted_courses %}
- 🎓 **[{{ course.title }}]({{ course.url }})**
  <br>📘 {{ course.description }}
  <br>🕒 Duration: {{ course.duration }}
  <br>🏁 Level: {{ course.level }}
  <br>
{% endfor %}

<ul>
  {% assign sorted_courses = site.courses | where_exp: "item", "item.exclude_from_course != true" | sort: "order" %}
  {% for course in sorted_courses %}
    <li>
      <a href="{{ course.url | absolute_url }}">{{ course.title }}</a>
    </li>
  {% endfor %}
</ul>
