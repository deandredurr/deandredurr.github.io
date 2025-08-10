---
layout: default
title: Essays
permalink: /essays/
---

# Essays
<ul class="list">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="meta">{{ post.date | date: "%b %d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
