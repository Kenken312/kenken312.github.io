---
layout: default
title: Music
permalink: /music/
---

## Music

曲数：{{ site.music.size }}

<ul>
{% assign items = site.music | sort_natural: "title" %}
{% for item in items %}
  <li>
    <a href="{{ item.url | relative_url }}">
      {{ item.title | escape }}
    </a>
    — {{ item.artist | escape }}
  </li>
{% endfor %}
</ul>
