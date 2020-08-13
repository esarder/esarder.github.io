---
layout: page
title: Art
permalink: /art/


---


<!-- <ul>
{% for tag in site.tags %}
  <li><a name="{{ tag | first }}">{{ tag | first }}</a>
    <ul>
    {% for post in tag.last %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
    </ul>
  </li>
{% endfor %}
</ul> -->


<link rel="stylesheet" type="text/css" media="all" href="/art/custom.css" />


<div class="panels">
  <div class="panels__container">
    <a href="music" class="panel" style="color:white">
      <div class="panel__content" style="background-image: url(guitar.jpg);">
      <h3 class="panel__title">Music</h3>
      </div>
    </a>
    <a href="photography" class="panel" style="color:white">
      <div class="panel__content" style="background-image: url(boulder_bum.jpg)">
      <h3 class="panel__title">Photography</h3>
      </div>
    </a>
    <a href="paint" class="panel" style="color:white">
      <div class="panel__content" style="background-image: url(oil_paints.jpg);">
      <h3 class="panel__title">Paint</h3>
      </div>
    </a>
  </div>
</div>
