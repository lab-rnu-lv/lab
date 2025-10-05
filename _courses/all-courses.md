---
layout: page
title: COURSES
exclude_from_course: true
---


# 📚 ROBOTICS

Here you can explore information and tasks for ROBOTICS students.

---

<div class="course-list">
  {% assign sorted_courses = site.courses | where_exp: "item", "item.exclude_from_course != true" | sort: "order" %}
  {% for course in sorted_courses %}
    <div class="course-card">
      <h2><a href="{{ site.baseurl }}{{ course.url }}">{{ course.title }}</a></h2>
      <p>{{ course.description }}</p>
      <p><strong>Deadline:</strong> {{ course.deadline }}</p>
    </div>
  {% endfor %}
</div>


