---
layout: post
title:  "Welcome to Yorkshire!"
date:   2016-06-13 10:51:47 +0530
categories: jekyll update
img: image-1.png
categories: [one, two]
---
First Time here..

Me too..  Lets see how long this lasts.

<div class="post-categories">
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
  <a href="{{site.baseurl}}/categories/{{category|slugize}}">{{category}}</a>
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>
