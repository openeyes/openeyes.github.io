---
permalink: "/news/"
layout: default
title:  "OpenEyes News"
---

<section id="feature-overview" style="background-color:#fff; padding-top:8em;">
      <div class="container">
        <div class="row">
          <div class="col-lg-10">
             <center><h2 class="section-heading">News</h2></center>
            <hr class="my-4">
               <p class="mb-0">
                {% for post in site.posts %}
                <div class="row form-group justify-content-md-center align-items-center">            
                  <div class="col-sm-5 center-block"><img  src="../{{ post.thumbnail }}" style="width:288px" alt="{{ post.title }}"></div>
                  <div class="col-sm-5 center-block"><b>{{ post.date | date: "%B %e, %Y" }}</b><br>{{ post.title }}<a class="btn" href="{{ post.url }}">More...</a></div>
                </div>
              {% endfor %}  
  