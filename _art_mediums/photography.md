---
title: Photography
layout: page
permalink: /art/photography/
---

{% for post in site.tags.photography %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
