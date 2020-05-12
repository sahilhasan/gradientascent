---
layout: page
title: Book Notes

---

<ul>
  {% for post in site.tags.books %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
