---
title: Making design data-informed
date: 2014-10-30 18:22:29 Z
categories:
- projects
layout: post
summary: This project is about how I make data-informed design decision by using A/B testing.
text: interface design, experimental design
thumbnail: https://res.cloudinary.com/ryanntt/image/upload/s--caXM7FiC--/c_scale,h_1082,w_1536/v1542723204/panelplace/panelplace-thumbnail.png
---

## Context

PanelPlace is a platform that helps people track and manage paid survey opportunities from market research companies. In July 2014, the client was working on significant feature changes and wanted to redesign the homepage as part of this rebranding. The conversion rate at homepage was low as people were reluctant to register for a new service like PanelPlace. As PanelPlace was growing its user base, therefore, this was the most critical issue on the website. The client wanted to take this opportunity to communicate with users about the rebranding of its product and new features.

<blockquote class="highlighted full-width">
    <h2 class="label">Reframed challenge</h2>
    <p>How can we redesign the homepage to convey trust and potential values of using PanelPlace to the new customers?</p>
</blockquote>

## Role

I worked together with Esther Fan, our user researcher in this project. I facilitated the ideation workshop, designed the homepage and conducted the experiment to measure the design.

<hr/>

## Problem research

### Competitive analysis

As new customers like to search for different alternatives before deciding which one to buy/use, we wanted to understand our competitor and therefore set our value proposition right so people can know which is unique about PanelPlace

My colleagues, Esther quickly did an analysis of competitors in the local market and how the website help them achieve their objectives. The client also discussed with us on how different they want to be from other competitors. 

### User research

We want to understand what people think when they reach the homepage, and why they don’t register for new account. This phase is to understand their needs and goals at the homepage. We asked them the following questions:

- How did you know about paid survey before joining PanelPlace?
- How did you earn money in the survey panels recommended by PanelPlace?
- What did you expect when signing up for PanelPlace?

We interviewed 6 users. The questions were structured to help us gain insights into their goals and needs in the platform. Some people joined the platform just because they had free time and want to spend on earning some money. Others are very systematic about how to manage their earning and want to be efficient when doing surveys. We identified a common theme among these users.

<blockquote class="highlighted full-width">
    <h2 class="label">Common theme</h2>
    <p>People consider answering surveys as a way to earn side money, so they do it only when the process is convenient, flexible and hassle-free.</p>
</blockquote>

<hr/>

## Ideation

### Co-design workshop with stakeholders

The early involvement of stakeholders in wireframing is essential to the faster approval of design later since stockholder will have a better sense of ownership in the design process. This project is the first time we experiment collaboration workshop with stakeholders. We wanted clients and designers to align themselves with each other about what the design will look like. 

<figure>
  <img src="/images/panelplace/collaboration-wireframe.jpg" alt="">
  <figcaption>We used Six Up method, which requires each person to draw 6 ideas. We then compiled and sorted them into catefories.</figcaption>
</figure>

<blockquote class="highlighted full-width">
    <h2 class="label">PanelPlace's Value Proposition</h2>
    <p>Our customers can focus on earning money as we help them choose and manage the optimal survey panels at their convenience.</p>
</blockquote>

## Experimental design

As the approval of design was mostly done by stakeholders previously, which explained why some design works were not successful after launch. We wanted to use data to assist decision making in choosing the best design.

As the objective of the homepage is to increase the rate of account registration, the key metrics of the homepage is the conversion rate measured by how many percentage people click the signup buttons in the form located at a few places in homepage. We started with a multivariate test for different changes at the signup form. Among all elements in the homepage, signup redesign has the most impact on changing the conversion rate.

### More communication of values and process

**Setup**

We wanted to know if simplifying the form, communicating more information of registration process would lead to a better conversion.

![Screenshots of control and variation]({{ site.url }}/images/panelplace/abtest-signup-form.jpg)


In the original homepage, the value of being secure was not well received by our interviewed users. Moreover, We used heatmap to monitor the homepage and found out that people rarely use the social media signup.

<figure>
  <img src="https://res.cloudinary.com/ryanntt/image/upload/s--bUrwzVDm--/c_scale,w_1536/v1542724481/panelplace/original-homepage.png" alt="" width="768">
  <figcaption>The original homepage communicated its value about security, had unnecessary elements such as the Facebook button.</figcaption>
</figure>

In the redesigned homepage, we conveyed the convenience of using PanelPlace by explaining the process of signing up. The form was simplified to contain only compulsory fields.

<figure>
  <img src="https://res.cloudinary.com/ryanntt/image/upload/s--UY7mACIw--/c_scale,w_1536/v1542724471/panelplace/redesigned-homepage.png" alt="" width="768">
  <figcaption>The redesigned homepage communicated its value about the ease of signing up and had a linear format of content leading to the form.</figcaption>
</figure>

**Result**

<table>
  <thead>
    <tr>
      <th>Version</th>
      <th>Conversion Rate</th>
      <th>Conversion</th>
      <th>Improvement</th>
    </tr>
  </thead>
  <tr>
    <td data-title="Design Version">Control</td>
    <td data-title="Conversion Rate">19.9%</td>
    <td data-title="Conversion">164/824</td>
    <td></td>
  </tr>
  <tr>
    <td data-title="Design Version">Variation</td>
    <td data-title="Conversion Rate">23.68%</td>
    <td data-title="Conversion">188/794</td>
    <td data-title="Improvement">+19.0% (97% confidence level)</td>
  </tr>
</table> 

![Result Graph]({{ site.url }}/images/panelplace/abtest-signup-form-graph.png)

### Clearer copy

**Setup**

After the experiment with main elements of the homepage, we decided to improve the signup button since it was the most prominent element in the signup form. In this experiment, we wanted to have more variations to validate against the control. 

![Screenshots of sign up button]({{ site.url }}/images/panelplace/abtest-signup-button.png)

There were one control and four variations. I ran the test for seven days. Within the first three days, two variations were lagging behind other variation, so I decided to stop traffic going through those variations. In the 5th day, another variation lagged far behind, and it was stopped due to its obvious non-improvement. In the 2nd variation, I saw a relative improvement of 14.8% at 96% confidence level within seven days.

**Result**

<table>
  <thead>
    <tr>
      <th>Version</th>
      <th>Conversion Rate</th>
      <th>Conversion</th>
      <th>Improvement</th>
    </tr>
  </thead>
  <tr>
    <td data-title="Version">Control</td>
    <td data-title="Conversion Rate">23.43%</td>
    <td data-title="Conversion">228/973</td>
    <td></td>
  </tr>
  <tr>
    <td data-title="Version">V1</td>
    <td data-title="Conversion Rate">26.90%</td>
    <td data-title="Conversion">244/907</td>
    <td data-title="Improvement">+14.80% (96% confidence level)</td>
  </tr>
  <tr>
    <td data-title="Version">V2</td>
    <td data-title="Conversion Rate">22.10%</td>
    <td data-title="Conversion">156/706</td>
    <td></td>
  </tr>
  <tr>
    <td data-title="Version">V3</td>
    <td data-title="Conversion Rate">20.61%</td>
    <td data-title="Conversion">128/621</td>
    <td></td>
  </tr>
  <tr>
    <td data-title="Version">V4</td>
    <td data-title="Conversion Rate">16.39%</td>
    <td data-title="Conversion">118/720</td>
    <td></td>
  </tr>
</table> 

![Result Graph]({{ site.url }}/images/panelplace/abtest-sginup-button-graph.png)


## Final result

Two weeks after we launched the redesigned homepage, the improvement of signup rate was relatively smaller than the result in the experiments. The reason, we agreed, was that the conversion rate was decided by not just individual elements but as a whole with their complex influential relationship. Regarding the time and traffic constraints we had, the testings helped my team improve the design, and convince client to implement the new design.  

<p style="color:#999999;">All information in this case study is my own and does not necessarily reflect PanelPlace's view.</p>
