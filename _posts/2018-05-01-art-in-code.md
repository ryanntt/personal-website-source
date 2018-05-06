---
title: Art in Code
date: 2018-05-01 08:06:18 Z
categories:
- projects
layout: post
status: 
text: How I play with art, technology and design
summary: Create generative art and game using Processing
thumbnail: https://res.cloudinary.com/ryanntt/image/upload/s--hNxdE9p6--/v1525530830/art-in-code/art-in-code-thumbnail.png
js: yes
---


> Are we the artists when the machines created by us draw artwork?


Above is the question I have when studying the Design Programming course in Master programme in University of Sydney. I have been convinced that the act of designing is to solve problems, therefore, creating a system that make design decision is also an act of designing. This is part of meta-design, which is a design approach that (re)design itself according to the problem at any given time. The philosophy beind metadesign is that future uses and problems cannot be completely known at design time, so we need to set certain constraint so that the designed system can evolve to adapt to new problems.

<hr>

### Artwork: Flow
*Static generative art*

The visual depicts the meeting moment of different **flows** coming from different directions. This phenomenon is seen in landscape such as waves of mountains, ocean. Different colours of flow represent different level of energy but belonging to the same type of nature. The scene may look harmonious or conflicting depending on how similar their directions and colour are when meeting each other. The colour of each variation represent a natural elements such as fire (red), water(blue), land(brown), tree(green), etc. Not all variations look visually harmonious, bringing to audience a wide variety of feeling.

*Please click the artwork to see new pattern*

<canvas style="margin-left:auto; margin-right: auto; display:block" data-processing-sources="/js/flow.pde"></canvas>

<hr>

### Artwork: Grid
*Animating generative art*

**Grid** is a collection of cells with different colours, similar to pixels on screens. Initially the grid has random colour pixels. A number of core cells are generated inside the grid with similar colours. Each of the core cells start spreading their hue, saturation and brightness to the different parts of grid and we can see how long does it take to dominate the whole space. Once a colour becomes dominant, the core cells are changed to a new colour and start spreading again. Grid represents a closeup view of pixels on screen, where we see millions of pixels from a distance. Any curve, gradient or any smooth visual are actually made of pixels with transitional colours. The concept was inspired by my interest in pixel art, LEGO bricks.

<canvas style="margin-left:auto; margin-right: auto; display:block" data-processing-sources="/js/grid.pde"></canvas>

<hr>

### Game: Galatic Run
*to be updated soon*