---
title: Ryan Nguyen - User Experience Designer in Sydney
layout: default
tag: home
---
<div class="intro" style="display:flex; align-items: flex-start;">

  <div class="avatar">
    <img src="./images/me.png"/>
  </div>

  <div  class="intro-text" style="">
    <h1> Hi, I'm Ryan.</h1>
    <p>I'm a UX/Product designer with five years of experience turning new technology and complex business to lovable products. Currently finishing my last semester of Master in Interaction Design at University of Sydney.</p>
    <p>Previously, I made travelling easier at <a href="https://www.wego.com" target="_blank">Wego</a>. My favourite part in design career has been building culture of collaborating and enabling each others to thrive in every team that I worked in. I love spending my time with talented people building <a href="#case-studies">meaningful products</a> together.</p> 
    <p>I am interested in designing for products that free up people from mundane tasks to have time for learning, family and life. Feel free to say hi if you want to collaborate on such products.</p>
    <p><a href="mailto:hello@ryanntt.com">hello@ryanntt.com</a></p>
    <form action="/pabot" style="display: inline-block; margin-right:0.5em">
      <input type="submit" class="button button-big mobile-block" value="Chat with Ryan's Avatar" />
    </form>

  </div>
</div>
<br/>

<h2 class="key-category" id="case-studies"> Case Studies</h2>

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
  <input type="submit" class="button button-big mobile-block" value="See all case studies" />
</form>


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