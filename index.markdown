---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<div>
  <img src="/photos/storm2.jpg" style="height:180px; width:fit-content" alt="storm_acomin"  class="center"/>
</div>

<h1 style="text-align:center; padding-top: 10px; font-weight:350;" class="home-header">Ella Sarder</h1>

<div class="wrapper">
  <p style="font-size:18px"> Ella is a student at the University of Colorado Boulder studying to receive her Bachelor of Science in Computer Science and a minor in Creative Technology and Design. She is interested in the ethics of how technology is developed and used, the benefits and repercussions of social media, and in teaching a more comprehensive basic understanding of technology to the general public. Ella strives to create a culture of personal responsibility among programmers for the application and possible consequences of the code they write.</p>
</div>

<br>

<div class="wrapper row">
  <div class="left col">
    <a href="resume" class="center rect_border" style="color:white"><span class="back_span">Resume</span></a>
  </div>

  <div class="right col">
    <a href="research" class="center rect_border" style="color:white"><span class="back_span">Research</span></a>
  </div>
</div>




{%- if site.posts.size > 0 -%}
<div class="wrapper" style="padding-top:30px">
  <h5 class="post-list-heading">{{ page.list_title | default: "Posts" }}</h5>
  <ul class="post-list">
    {%- for post in site.posts -%}
    <li>
      {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h5>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h5>
      {%- if site.show_excerpts -%}
        {{ post.excerpt }}
      {%- endif -%}
    </li>
    {%- endfor -%}
  </ul>

{%- endif -%}
</div>


<style>

  .back_span{
    background-color: #393939;
    padding: 7px 12px 7px 12px;
    border-radius: 2px;
  }

  .rect_border{
    text-align:center;
    font-size:20px;
    color: white;
  }

  .col {
    float: left;
    padding: 10px;
    vertical-align: middle;  

  }

  .left {
    width: 50%;
  }

  .right {
    width: 50%;
  }

  .row {
    display: flex;
  }

  .center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  }

  .trigger{
    padding-top:16px;
  }

  .post-list-heading {
    font-size: 22px;
  }

  .post-link {
    font-size: 18px;
  }

  .page-content{
    padding: 0px 0px 30px 0px;
  }

  p {
    font-size:18px;
  }


  .home-header {
  @include relative-font-size(1.625);
  font-weight: 300;
  letter-spacing: -1px;

}


</style>
