---
title: Music
layout: page
permalink: /art/music/
---

{% for post in site.tags.music %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
