---
layout: page
title: Tech Posts

---

<ul>
  {% for post in site.tags.tech %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
