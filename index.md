---
title: Ryan Nguyen - User Experience Designer in Sydney
layout: default
tag: home
---
<section class="intro">

  <div class="switch theme-toggle-button">
    <input class="switch__input" type="checkbox" id="theme-toggle" onclick="modeSwitcher()">
    <label class="switch__label" for="theme-toggle">Dark Mode</label>
    <div aria-hidden="true" class="switch__marker" id="theme-label"></div>
  </div>
  <div  class="intro-text">
    <h1> Hello, I'm Ryan, a product designer in Sydney. I design meaningful and lovable products across different technologies and businesses.</h1>
    <form>
      <input id="start-chat" type="button" class="button button-big mobile-block" value="Feeling chatty today" onClick="startChat()"/>
    </form>
    <div class="spacer-block-2"></div>
  </div>
  <div id="chat" class="hidden">
    <div class="botui-app-container" id="my-pa">
      <div id="avatar" class="hidden">
        <img src="./images/me.png" alt="">    
      </div>
      <bot-ui></bot-ui>
    </div>
  </div>
</section>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="h1 key-category" id="case-studies">Select Case Studies</h2>

  <div class="projects list featured">
    <div class="posts">
      {% for post in site.categories.projects %}
        {% if post.status contains 'featured' %}
          <div class="post-entry py3">
            <div class="summary">
              <a href="{{ post.url | prepend: site.baseurl }}">
                <h2 class="h2 title">{{ post.title }}</h2>
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
            <a href="{{ post.url | prepend: site.baseurl }}" class="thumbnail">
              <div class="wrap">
                <img class="thumb" src="{{ post.thumbnail }}" ref="{{ post.title | downcase | prepend: site.baseurl }}" alt="{{post.title}}">  
              </div>
            </a>
          </div>
        {% endif %}
      {% endfor %}
    </div>
  </div>

</section>

<div class="spacer-block-1"></div>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="h1 key-category">Writings</h2>

  <div class="blog featured">
    <div class="posts">
      {% for post in site.categories.blog limit:3 %}
        <div class="post py3">
          <a href="{{ post.url | prepend: site.baseurl }}"><h3 class="h3 post-title">{{ post.title }}</h3></a>
          <p class="post-summary">
            {% if post.summary %}
              {{ post.summary }}
            {% else %}
              {{ post.excerpt }}
            {% endif %}
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">Read more</a>
          </p>
        </div>
      {% endfor %}
    </div>
  </div>

</section>

<div class="spacer-block-1"></div>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="h1 key-category">Message Ryan</h2>
  <p style="max-width: 650px;">If you'd like to have a chat, please send me an email at <a href="mailto:{{ site.email }}">{{ site.email }}</a> and I will reply shortly.</p>
</section>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
<script src="./js/vue/2.0.6/vue.min.js"></script>
<script src="./js/botui/botui.min.js"></script>
<script src="./js/botui/mybot.js"></script>