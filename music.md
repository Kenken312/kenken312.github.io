---
layout: default
title: Music
permalink: /music/
---

# Music

テスト

<ul>
{% assign items = site.music | sort: "date" | reverse %}
{% for item in items %}
  <li>
    <a href="{{ item.url | relative_url }}">
      {{ item.title | escape }}
    </a>
    — {{ item.artist | escape }}
  </li>
{% endfor %}
</ul>
