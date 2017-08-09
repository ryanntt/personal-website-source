---
title: Projects
layout: default
tag: projects
---

### Key Projects
<div class="projects list">
  <div class="posts">
    {% for post in site.categories.projects %}
      {% if post.status contains 'featured' %}
        <div class="post-entry py3">
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
            <div class="wrap">
              <div class="summary">
                <h3 class="h1 title">{{ post.title }}</h3>
                <p class="text">
                {% if post.text %}
                  {{ post.text }}
                {% endif %}
                </p>
              </div>
              <img class="thumb" src="{{ post.thumbnail }}" ref="{{ post.title | downcase | prepend: site.baseurl }}" alt="{{post.title}}">  
            </div>
          </a>
        </div>
      {% endif %}
    {% endfor %}
  </div>
</div>

------

### Other Projects
<div class="projects list">
  <div class="posts">
    {% for post in site.categories.projects %}
        {% if post.status contains 'featured' %}
        {% else %}
          <div class="post py3">
            <a href="{{ post.url | prepend: site.baseurl }}" class="post-link"><h3 class="h2 post-title">{{ post.title }}</h3></a>
            <p class="post-summary">
              {% if post.summary %}
                {{ post.summary }}
              {% else %}
                {{ post.excerpt }}
              {% endif %}
            </p>
          </div>
        {% endif %}
    {% endfor %}
  </div>
</div>