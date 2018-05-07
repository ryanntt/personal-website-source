---
title: Ryan Nguyen - User Experience Designer in Sydney
layout: default
tag: home
---

# Hi, I'm Ryan.

## I'm a user experience and product designer.

👨‍🎓 I'm studying Master of Interaction Design and Electronic Arts in University of Sydney, Australia. Previously, I worked for [Wego](https://www.wego.com), a travel tech company, as a designer in Web Experience team.

Want to know more about me? Have a chat 💬 with [my digital avatar](https://ryanntt.com/pabot).

<p style="margin-bottom:0;">You can contact me through:</p>

<small>
  <a target="_blank" class="no-underline" href="http://linkedin.com/in/ryanntt">
    <span class="fa-stack fa-lg">
      <i class="fa fa-linkedin" aria-hidden="true"></i>
    </span>
  </a>
  <a class="no-underline" href="/contact">
    <span class="fa-stack fa-lg">
      <i class="fa fa-envelope-o" aria-hidden="true"></i>
    </span>
  </a>
</small>

<h2 class="key-category"> Key Projects</h2>

<div class="projects list featured">
  <div class="posts">
    {% for post in site.categories.projects %}
      {% if post.status contains 'featured' %}
        <div class="post-entry py3">
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
            <div class="wrap">
              <img class="thumb" src="{{ post.thumbnail }}" ref="{{ post.title | downcase | prepend: site.baseurl }}" alt="{{post.title}}">  
            </div>
          </a>
          <div class="summary">
            <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
              <h3 class="h2 title">{{ post.title }}</h3>
            </a>
            <p class="text">
              {% if post.text %}
                {{ post.text }}
              {% endif %}
            </p>
          </div>
        </div>
      {% endif %}
    {% endfor %}
  </div>
</div>

<form action="/projects" class="center">
  <input type="submit" class="button button-big mobile-block" value="See all projects" />
</form>


<h2 class="key-category">Writing</h2>

<div class="blog featured">
  <div class="posts">
    {% for post in site.categories.blog limit:3 %}
      <div class="post py3">
        <a href="{{ post.url | prepend: site.baseurl }}" class="post-link"><h3 class="h3 post-title">{{ post.title }}</h3></a>
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

<form action="/blog" class="center">
  <input type="submit" class="button button-big mobile-block" value="See all writings" />
</form>