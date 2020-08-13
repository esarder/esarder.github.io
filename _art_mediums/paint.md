---
title: Paint
layout: page
permalink: /art/paint/
---

{% for post in site.tags.paint%}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
