---
title: Ryan Nguyen - User Experience Designer in Sydney
layout: default
tag: home
---

# Hi, I'm Ryan, designer for products and interaction.

I'm studying Master of Interaction Design and Electronic Arts in University of Sydney, Australia.

Previously, I worked in Singapore for [Wego](http://www.wego.com) as a designer in Web Experience team. 

--------

### Key Projects

<div class="projects list featured">
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

[See All Projects](/projects)