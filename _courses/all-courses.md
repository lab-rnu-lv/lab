---
layout: page
title: COURSES
exclude_from_course: true
---

<ul>
  {% assign sorted_courses = site.courses | where_exp: "item", "item.exclude_from_course != true" | sort: "order" %}
  {% for course in sorted_courses %}
    <li>
      <a href="{{ course.url | absolute_url }}">{{ course.title }}</a>
    </li>
  {% endfor %}
</ul>
