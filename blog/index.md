---
title: Writings
layout: default
pagination: 
  enabled: true
  category: blog
  permalink: '/:num/'
---
<div class="blog">
  <div class="posts">
    {% for post in paginator.posts %}
      <div class="post py3">
        <p class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</p>
        <a href="{{ post.url | prepend: site.baseurl }}"><h3 class="h2 post-title">{{ post.title }}</h3></a>
        <p class="post-summary">
          {% if post.summary %}
            {{ post.summary }}
          {% else %}
            {{ post.excerpt }}
          {% endif %}
        </p>
      </div>
    {% endfor %}
  </div>
</div>

{% include pagination.html %}
