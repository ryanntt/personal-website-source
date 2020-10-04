---
title: Case Studies
layout: default
tag: projects
---

<div class="projects list">
  <div class="posts">
    {% for post in site.categories.projects %} 
      <a href="{{ post.url | prepend: site.baseurl }}">
        <div class="post py2">
          <div class="summary">
            <h3 class="h2 post-title">{{ post.title }}</h3>
            <p class="text">
              {% if post.text %}
                {{ post.text }}
              {% endif %}
            </p>
          </div>
          <div class="thumbnail">
            <div class="wrap">
              {% cloudinary thumb {{ post.thumbnail }} alt="{{post.title}}" %}
            </div>
          </div>
        </div>
      </a>
    {% endfor %}
  </div>
</div>