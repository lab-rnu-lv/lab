---
layout: page
title: COURSES
exclude_from_course: true
---


# 📚 Available Courses

Welcome to our course list!  
Here you can explore all available topics sorted by category.

---

<h1>🎓 Course Catalog</h1>
<p>Explore our latest modules and lessons below.</p>

<div class="course-list">
  {% assign sorted_courses = site.courses | where_exp: "item", "item.exclude_from_course != true" | sort: "order" %}
  {% for course in sorted_courses %}
    <div class="course-card">
      <h2><a href="{{ site.baseurl }}{{ course.url }}">{{ course.title }}</a></h2>
      <p>{{ course.description }}</p>
      <p><strong>Duration:</strong> {{ course.duration }}</p>
    </div>
  {% endfor %}
</div>


