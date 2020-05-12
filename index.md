---
layout: page
title: Gradient Ascent

---

### Most Recent Posts! 
<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>, posted on <time>{{post.date | date: "%-d %B %Y" }}</time>
    </li>
  {% endfor %}
</ul>

<br>

### Tags
<ul>
  {% assign sorted_tags = site.tags | sort %}
  {% for tag in sorted_tags %}
    {% assign t = tag | first %}
    {% assign posts = tag | last %}
    <li>
      <a href="/{{ t | downcase | replace:' ','-'}}">
        {{t | downcase | replace:' ','-' }}
        <span>({{ posts | size }})</span>
      </a>
    </li>
  {% endfor %}
</ul>


