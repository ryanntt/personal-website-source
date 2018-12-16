---
title: Ryan Nguyen - User Experience Designer in Sydney
layout: default
tag: home
---
<section class="intro">

  <!-- <div class="horizontal-bar"></div> -->
  <div  class="intro-text">
    <h1> Hello, I'm Ryan, a product designer in Sydney. I design meaningful and lovable products across different technologies and businesses.</h1>
    <form>
      <input id="start-chat" type="button" class="button button-big mobile-block" value="Feeling Chatty Today" onClick="startChat()"/>
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
  <h2 class="h1 key-category" id="case-studies"> Case Studies</h2>

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
  <h2 class="h1 key-category">Work with Ryan</h2>
  <p style="max-width: 650px;">I'm looking for a challenging role in which I can use my skill sets and creativity to add values to the business and users. If you want to work together, please fill in the following form and I will reply shortly.</p>

  <div class="py2" style="max-width: 650px;">
    {% if site.ajaxify_contact_form %}
      <form class="form-stacked">
        <input type="text" name="email" class="field-light" placeholder="Your email address">
        <textarea type="text" name="content" class="field-light" rows="5" placeholder="What would you like to say?"></textarea>
        <input type="hidden" name="_subject" value="New submission!" />
        <input type="text" name="_gotcha" style="display:none" />
        <button type='submit' class="button button-big mobile-block" >Send to Ryan</button>
      </form>
    {% else %}
      <form action="https://formspree.io/{{ site.email }}" method="POST" class="form-stacked">
        <input type="text" name="email" class="field-light" placeholder="Your email address">
        <textarea type="text" name="content" class="field-light" rows="5" placeholder="What would you like to say?"></textarea>
        <input type="hidden" name="_next" value="{{ site.baseurl }}/thanks/" />
        <input type="hidden" name="_subject" value="New submission!" />
        <input type="text" name="_gotcha" style="display:none" />
        <input type="submit" class="button button-big mobile-block" value="Send to Ryan">
      </form>
    {% endif %}
  </div>
</section>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
<script src="./js/vue/2.0.6/vue.min.js"></script>
<script src="./js/botui/botui.min.js"></script>
<script src="./js/botui/mybot.js"></script>