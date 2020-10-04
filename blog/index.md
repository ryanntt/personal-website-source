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
      <a href="{{ post.url | prepend: site.baseurl }}">
        <div class="post py2">
          <p class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</p>
          <h3 class="h3 post-title">{{ post.title }}</h3>
          <p class="post-summary">
            {% if post.summary %}
              {{ post.summary }}
            {% else %}
              {{ post.excerpt }}
            {% endif %}
          </p>
        </div>
      </a>
    {% endfor %}
  </div>
</div>

{% include pagination.html %}
