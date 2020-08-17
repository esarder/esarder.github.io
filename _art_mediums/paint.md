---
title: Paint
layout: page
permalink: /art/paint/
---


{% for post in site.tags.paint %}
  <div class="content ">
    <img src="{{ post.thumbnail }}" alt="{{ post.title}}" height="300" width="400">
    <a class="text" href="{{ post.url }}" style="color:black">{{ post.title }}</a>
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
  color: black;
}

.text {
  position: absolute;
  top: 50%;
  text-size: 18px;
  left: 50%;
  background-color: rgba(280, 280, 280, 0.85);
  transform: translate(-50%, -50%);
  color: black;
  padding: 20px;
}



</style>
