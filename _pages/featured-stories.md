---
permalink: "/featured-stories/"
layout: singlePage
title:  "Featured Stories"
---



<section class="text-white" id="news" style="background-color:#1a5281">
      <div class="container text-center">
      <div class="col-lg-10 mx-auto">
              <h2 class="mb-4">Featured Stories</h2>
       <hr class="my-4"> 
        <div class="row"> 
              <div class="row" id="stories">
               {% for post in site.posts %}
                <div class="col-md-4">
                  <div class="thumbnail">
                  <a href="{{ post.url }}">
                  <img  src="{{ post.thumbnail }}" style="width:100%" alt="{{ post.title }}">
                  <div class="caption text-white"><br>
                    <p>{{ post.title }}</p> 
                  </div>
                  </a>
                </div>
                </div>
              {% endfor %}
              </div>
        </div>
       </div>
    </div>
</section>
  