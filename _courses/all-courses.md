---
layout: course
title: all-courses
exclude_from_course: true
---

<ul>
  {% assign sorted_courses = site.courses | sort: "order" %}
  {% for course in sorted_courses %}
    <li>
      <a href="{{ course.url | absolute_url }}">{{ course.title }}</a> 
    </li>
  {% endfor %}
</ul>
