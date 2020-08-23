---
title: Paint
layout: page
permalink: /art/paint/
---


{% for post in site.tags.paint %}
  <div class="content ">
    <img class="img_thumb" src="{{ post.thumbnail }}" alt="{{ post.title}}">
    <a class="text" href="{{ post.url }}" style="color:black">{{ post.title }}</a>
  </div>
{% endfor %}


<style>
.img_thumb {
  height: 300px;
  width: 400px;
}

.content {
  position: relative;
  width: 400px;
  height: 300px;
  padding: 10px
}

a:hover {
  color: white;
}

.text {
  text-align: center;
  position: absolute;
  top: 50%;
  font-size: 18px;
  left: 50%;
  background-color: rgba(255, 255, 255, 0.85);
  transform: translate(-50%, -50%);
  color: black;
  padding: 20px;
}

@media only screen and (max-width: 600px) {
  .img_thumb{
    height: 200px;
    width: 264px;
  }

  .content {
    height: 200px;
    width: 264px;
  }

  .text {
    font-size: 14px;
    padding: 10px;
  }
}
</style>
