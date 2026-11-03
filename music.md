---
layout: default
title: Music
permalink: /music/
---

## Music

登録されている曲数：{{ site.music.size }}

<ul>
{% for item in site.music %}
  <li>
    <a href="{{ item.url | relative_url }}">
      {{ item.title | escape }}
    </a>
  </li>
{% endfor %}
</ul>
