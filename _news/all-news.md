---
layout: page
title: NEWS
---

<ul>
  {% assign sorted_news = site.news | sort: "date" | reverse %}
  {% for news in sorted_news %}
    <li>
      <a href="{{ news.url | relative_url }}">{{ news.title }}</a> — {{ news.date | date: "%d.%m.%Y" }}
    </li>
  {% endfor %}
</ul>
