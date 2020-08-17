---
title: Photography
layout: page
permalink: /art/photography/
---

{% for post in site.tags.photography %}
  <div class="content ">
    <img src="{{ post.thumbnail }}" alt="{{ post.title}}" height="400" width="500">
    <a class="text" href="{{ post.url }}" style="color:white">{{ post.title }}</a>
  </div>
{% endfor %}



<style>

.content {
  text-align: center;
  position: relative;
  width: 500px;
  height: 400px;
  padding: 10px
}

a:hover {
        color: white;
}

.text {
  position: absolute;
  top: 50%;
  text-size: 18px;
  left: 50%;
  background-color: rgba(0, 0, 0, 0.85);
  transform: translate(-50%, -50%);
  color: white;
  padding: 20px;
}



</style>
