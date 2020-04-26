---
layout: post
title: Main

---

# Whats up!

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>



<section>

    <h2>Tags</h2>
    <ul>
      {% assign sorted_tags = site.tags | sort %}
      {% for tag in sorted_tags %}
        {% assign t = tag | first %}
        {% assign posts = tag | last %}
        <li>
          <a href="/tags/# {{ t | downcase | replace:' ','-'}}">
            {{t | downcase | replace:' ','-' }}
            <span>({{ posts | size }})</span>
          </a>
        </li>
      {% endfor %}
    </ul>

</section>

