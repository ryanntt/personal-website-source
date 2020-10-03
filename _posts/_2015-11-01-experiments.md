---
title: Experimental works
date: 2015-11-01 18:03:18 Z
original_date: 2015-11-01 08:06:18 Z
categories:
- projects
layout: page
status: featured
text:  <span>Interaction design</span> <span>Animation</span> <span>Coding</span>
summary: <p>I like to spend my free time in experimenting new UI, features and products.</p>
year: 2015 - 2019
theme-color: 888888
thumbnail: https://res.cloudinary.com/ryanntt/image/upload/s--Xc5h1P6---/v1525614090/art-in-code/art-in-code-thumbnail.png
custom-javascript-list:
- "https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"
- "/js/processing.min.js"
---

These are some of my experimental works on interface design, animation and computing art. 

<figure class="no-bg text-width">
  <canvas style="margin-left:auto; margin-right: auto; display:block" data-processing-sources="/js/flow.pde"></canvas>
  <figcaption>
  <b>Flow (2017)</b>: The artwork depicts the meeting moment of different flows coming from different directions. This phenomenon is seen in landscape such as waves of mountains, rivers and ocean waves. Different colours of flow represent different levels of energy but belonging to the same type of natural element. The scene may look harmonious or conflicting depending on how similar their directions and colours are when meeting each others. The colour of each variation represents a natural element such as fire (red), water(blue), land(brown), tree(green), etc. Not all variations look visually harmonious, bringing to audience a wide variety of feelings and interpretations.<br>

  <em>Please click the artwork to see new pattern.</em>
  </figcaption>
</figure>

<figure class="no-bg text-width">
  <canvas style="margin-left:auto; margin-right: auto; display:block" data-processing-sources="/js/grid.pde"></canvas>
  <figcaption>
  <b>Grid (2017)</b>: This is a collection of cells with different colours, similar to pixels on screens. Initially the grid has random colour pixels. A number of core cells are generated inside the grid with similar colours. Each of the core cells start spreading their hue, saturation and brightness to the different parts of grid and we can see how long does it take to dominate the whole space. Once a colour becomes dominant, the core cells are changed to a new colour and start spreading again. Grid represents a closeup view of pixels on screen, where we see millions of pixels from a distance. Any curve, gradient or any smooth visual are actually made of pixels with transitional colours. The concept was inspired by my interest in pixel art, LEGO bricks, and the emergent character of natural and social phenemnons such as diseases and cultural domination. 
  </figcaption>
</figure>


<hr>

<div id="shots"></div>

<script>
//Set the Access Token
var accessToken = "9daf27d240782089f50bfaa2d51b522a94c818bf7602993dd63257eb5feca9d4";

//Call Dribbble v2 APi
$.ajax({
    url: 'https://api.dribbble.com/v2/user/shots?per_page=8&access_token='+accessToken,
    dataType: 'json',
    type: 'GET',
    success: function(data) {  
      if (data.length > 0) { 
        $.each(data.reverse(), function(i, val) {
          // Display shots that have tag "ui"
          if (val.tags.indexOf("ui")>-1) {
            $('#shots').prepend(
            '<figure class="no-bg-color text-width" target="_blank" href="'+ val.html_url +'" title="' + val.title + '"><img src="'+ val.images.hidpi +'"/><figcaption>' + val.title + '</figcaption></figure>'
            )
          }                
        })
      }
      else {
        $('#shots').append('<p>No shots yet!</p>');
      }
    }
});
</script>





