---
title: Case Studies
layout: default
tag: projects
---

## Case Studies
<div class="projects list">
  <div class="posts">
    {% for post in site.categories.projects %} 
        <div class="post-entry py3">
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
            <div class="wrap">
              <img class="thumb" src="{{ post.thumbnail }}" ref="{{ post.title | downcase | prepend: site.baseurl }}" alt="{{post.title}}">  
            </div>
          </a>
          <div class="summary">
            <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
              <h3 class="h3 title">{{ post.title }}</h3> 
            </a>
              <p class="text">
              {% if post.text %}
                {{ post.text }}
              {% endif %}
              </p>
          </div>
        </div>
    {% endfor %}
  </div>
</div>