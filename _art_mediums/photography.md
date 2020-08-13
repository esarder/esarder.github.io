---
title: Photography
layout: page
permalink: /art/photography/
---

{% for post in site.tags.photography %}
 <li> <a href="{{ post.url }}">{{ post.title }}</a> &nbsp;- <span>{{ post.date | date_to_string }}</span> </li>
{% endfor %}
