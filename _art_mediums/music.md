---
title: Music
layout: page
permalink: /art/music/
---

{% for post in site.tags.music %}
  <div class="content ">
    <img src="{{ post.thumbnail }}" alt="{{ post.title}}" height="300" width="400">
    <a class="text" href="{{ post.url }}" style="color:white">{{ post.title }}</a>
  </div>
{% endfor %}


<style>

.content {
  text-align: center;
  position: relative;
  width: 400px;
  height: 300px;
  padding: 10px
}

a:hover {
        color: white;
}

.text {
  position: absolute;
  top: 50%;
  text-size: 18px
  left: 50%;
  background-color: rgba(0, 0, 0, 0.85);
  transform: translate(-50%, -50%);
  color: white;
  padding: 20px;
}



</style>
