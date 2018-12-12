---
title: Ryan Nguyen - User Experience Designer in Sydney
layout: default
tag: home
---
<section class="intro">

  <div class="horizontal-bar"></div>
  <div  class="intro-text">
    <h1> Hello, I'm Ryan, a product designer in Sydney. I design meaningful and lovable products across different technologies and businesses.</h1>
    <form action="/pabot">
      <input type="submit" class="button button-big mobile-block" value="Feeling chatty today ?" />
    </form>
  </div>
</section>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="key-category" id="case-studies"> Case Studies</h2>

  <div class="projects list featured">
    <div class="posts">
      {% for post in site.categories.projects %}
        {% if post.status contains 'featured' %}
          <div class="post-entry py3">
            <div class="summary">
              <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
                <h3 class="h2 title">{{ post.title }}</h3>
              </a>
              <p class="text">
                {% if post.text %}
                  {{ post.text }}
                {% endif %}
              </p>
              <a href="{{ post.url | prepend: site.baseurl }}" class="post-link">
                View case study
              </a>
            </div>
            <a href="{{ post.url | prepend: site.baseurl }}" class="post-link thumbnail">
              <div class="wrap">
                <img class="thumb" src="{{ post.thumbnail }}" ref="{{ post.title | downcase | prepend: site.baseurl }}" alt="{{post.title}}">  
              </div>
            </a>
          </div>
        {% endif %}
      {% endfor %}
    </div>
  </div>

  <form action="/projects" class="center">
    <input type="submit" class="button button-big mobile-block" value="See all case studies" />
  </form>
</section>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="key-category">Writings</h2>

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
</section>