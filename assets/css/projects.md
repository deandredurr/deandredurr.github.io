---
layout: default
title: Projects
permalink: /projects/
---

# Projects
<div class="grid">
{% for project in site.projects %}
<article class="card">
  <a href="{{ project.url | relative_url }}">
    {% if project.thumb %}<img src="{{ project.thumb | relative_url }}" alt="">{% endif %}
    <h3>{{ project.title }}</h3>
    <div class="meta">
      {% if project.year %}{{ project.year }}{% endif %}
      {% if project.role %} • {{ project.role }}{% endif %}
    </div>
  </a>
</article>
{% endfor %}
</div>
