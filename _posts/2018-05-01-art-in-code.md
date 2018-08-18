---
title: Art in Code
date: 2018-05-01 08:06:18 Z
categories:
- projects
layout: post
text: How I play with art, technology and design
summary: Create generative art and game using Processing
thumbnail: https://res.cloudinary.com/ryanntt/image/upload/s--Xc5h1P6---/v1525614090/art-in-code/art-in-code-thumbnail.png
js: yes
---


> Are we the artists when the machines created by us draw artwork?


Above is the question I had when studying the Design Programming course in Master programme in University of Sydney. To design is to solve problems, therefore, creating a system that makes design decision is also designing. This is part of meta-design, which is a design approach that (re)designs itself according to the problem at any given time. The philosophy behind metadesign is that future uses and problems cannot be completely known at design time, so we need to set certain constraint and the designed system will evolve to adapt to new problems.

<hr>

### Artwork: Flow
*Static generative art*

The artwork depicts the meeting moment of different **flows** coming from different directions. This phenomenon is seen in landscape such as waves of mountains, rivers and ocean waves. Different colours of flow represent different levels of energy but belonging to the same type of natural element. The scene may look harmonious or conflicting depending on how similar their directions and colours are when meeting each others. The colour of each variation represents a natural element such as fire (red), water(blue), land(brown), tree(green), etc. Not all variations look visually harmonious, bringing to audience a wide variety of feelings and interpretations.

*Please click the artwork to see new pattern*

<canvas style="margin-left:auto; margin-right: auto; display:block" data-processing-sources="/js/flow.pde"></canvas>

<hr>

### Artwork: Grid
*Animating generative art*

**Grid** is a collection of cells with different colours, similar to pixels on screens. Initially the grid has random colour pixels. A number of core cells are generated inside the grid with similar colours. Each of the core cells start spreading their hue, saturation and brightness to the different parts of grid and we can see how long does it take to dominate the whole space. Once a colour becomes dominant, the core cells are changed to a new colour and start spreading again. Grid represents a closeup view of pixels on screen, where we see millions of pixels from a distance. Any curve, gradient or any smooth visual are actually made of pixels with transitional colours. The concept was inspired by my interest in pixel art, LEGO bricks, and the emergent character of natural and social phenemnons such as diseases and cultural domination. 

<canvas style="margin-left:auto; margin-right: auto; display:block" data-processing-sources="/js/grid.pde"></canvas>

<hr>

### Game: Galatic Run
*to be updated soon*