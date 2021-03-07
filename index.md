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
        {% cloudinary avatar /images/me.png alt="Ryan Nguyen" %}
      </div>
      <bot-ui></bot-ui>
    </div>
  </div>
</section>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="h1 key-category mr1" id="case-studies">Select Case Studies</h2>
  <a class="link" href="{{ site.baseurl }}/projects/">View all</a>
  <div class="projects list featured">
    <div class="posts">
      {% for post in site.categories.projects %}
        {% if post.status contains 'featured' %}
          <a href="{{ post.url | prepend: site.baseurl }}">
            <div class="post py2">
              <div class="summary">
                  <h2 class="h2 post-title">{{ post.title }}</h2>
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
        {% endif %}
      {% endfor %}
    </div>
  </div>
</section>

<div class="spacer-block-1"></div>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="h1 key-category mr1">Publications</h2>
  <div class="blog">
    <div class="publication">
      <div class="posts">
        <a class="link" href="https://dl.acm.org/doi/abs/10.1145/3342197.3344543" target="_blank">
          <div class="post py2">
            <h3 class="h4 post-title">
              Designing for Projection-based Communication between Autonomous Vehicles and Pedestrians. 
            </h3>
            <p class="summary">
              <span><em>Nguyen, Trung Thanh</em>, Kai Holländer, Marius Hoggenmueller, Callum Parker, and Martin Tomitsch</span>
              <span>11th International Conference on Automotive User Interfaces and Interactive Vehicular Applications</span>
              <span>September 2019</span>
              <span>Pages 284-294</span>
            </p>
          </div>
        </a>
        <a class="link" href="https://dl.acm.org/doi/abs/10.1145/3441000.3441031" target="_blank">
          <div class="post py2">
            <h3 class="h4 post-title">
              Tangible Multi-Display Toolkit to Support the Collaborative Design Exploration of AV-Pedestrian Interfaces 
            </h3>
            <p class="summary">
              <span>Marius Hoggenmueller, Martin Tomitsch, Callum Parker, <em>Trung Thanh Nguyen</em>, Dawei Zhou, Stewart Worrall, Eduardo Nebot</span>
              <span>32nd Australian Conference on Human-Computer Interaction</span>
              <span>December 2020</span>
              <span>Pages 25-35</span>
            </p>
          </div>
        </a>
      </div>
    </div>
  </div>
</section>

<div class="spacer-block-1"></div>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="h1 key-category mr1">Writings</h2>
  <a class="link" href="{{ site.baseurl }}/blog/">View all</a>

  <div class="blog featured">
    <div class="posts">
      {% for post in site.categories.blog limit:3 %}
        <a href="{{ post.url | prepend: site.baseurl }}">
          <div class="post py1">
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
</section>

<div class="spacer-block-1"></div>

<section>
  <div class="horizontal-bar"></div>
  <h2 class="h1 key-category">Message Ryan</h2>
  <p style="max-width: 650px;">If you'd like to have a chat, please send me an email at <a href="mailto:{{ site.email }}" class="link">{{ site.email }}</a> and I will reply shortly.</p>
</section>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
<script src="./js/vue/2.0.6/vue.min.js"></script>
<script src="./js/botui/botui.min.js"></script>
<script src="./js/botui/mybot.js"></script>