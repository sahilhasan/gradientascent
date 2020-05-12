---
layout: page
title: Misc Posts

---

<ul>
  {% for post in site.tags.misc %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
