---
title: Case Studies
layout: default
tag: projects
---

<div class="projects list">
  <div class="posts">
    {% for post in site.categories.projects %} 
      <div class="post py3">
        <div class="summary">
          <a href="{{ post.url | prepend: site.baseurl }}">
            <h3 class="h2 post-title">{{ post.title }}</h3>
          </a>
          <p class="text">
            {% if post.text %}
              {{ post.text }}
            {% endif %}
          </p>
        </div>
        <a href="{{ post.url | prepend: site.baseurl }}" class="thumbnail">
          <div class="wrap">
            <img class="thumb" src="{{ post.thumbnail }}" ref="{{ post.title | downcase | prepend: site.baseurl }}" alt="{{post.title}}">  
          </div>
        </a>
      </div>
    {% endfor %}
  </div>
</div>