---
layout: page
title: Art
permalink: /art/
---

Placeholder for art page.

{% for medium in site.art_mediums %}
  <h2>
    <a href="{{ medium.url }}">
      {{ medium.title }}
    </a>
  </h2>
  <p>{{ medium.content | markdownify }}</p>
{% endfor %}


![Boy and a Boulder](boulder_bum.jpg)
