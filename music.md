---
layout: default
title: Music
permalink: /music/
---

## Music

好きな音楽について、感想を書いています。

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
