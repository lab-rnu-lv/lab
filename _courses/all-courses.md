---
layout: page
title: all-courses
---

<ul>
  {% assign sorted_courses = site.courses | sort: "order" %}
  {% for course in sorted_courses %}
    <li>
      <a href="{{ course.url | absolute_url }}">{{ course.title }}</a> 
    </li>
  {% endfor %}
</ul>
