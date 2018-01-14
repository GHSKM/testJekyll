---
layout: default
title: Posts TWS
permalink: /blog/
---
<div class="row">

  {% for post in site.categories.featured limit: 3 %}
  <div class="col-md-4">
    <div class="main-post">
      <a href="{{ post.url | prepend: site.baseurl }}" class="main-post-title">{{ post.title }}</a>
      <span>{{ post.date | date: '%B %d, %Y' }}</span>

      <div class="main-thumb">
        <a href="{{ post.url | prepend: site.baseurl }}"><img src="/images/{{ post.thumb }}" /></a>
      </div>

      <p>{{ post.description }}</p>
    </div>
  </div>
  {% endfor %}

</div>
