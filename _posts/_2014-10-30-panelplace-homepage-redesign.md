---
title: PanelPlace
date: 2014-10-30 18:22:29 Z
categories:
- projects
layout: post
summary: This project is about how I learnt A/B testing and first time experienced
  product development process
text: Homepage optimisation using A/B testing
thumbnail: https://res.cloudinary.com/ryanntt/image/upload/s--hyRorDuK--/c_scale,w_768/v1506611885/panelplace/thumbnail.png
---

This project is about how I learnt A/B testing and first time experienced product development process. 

## Project Overview

PanelPlace is a platform that helps people track and manage paid survey opportunities from market research companies. 

### Project Challenges
In July 2014, the client was working on major feature changes and want to redesign the homepage as part of rebranding. The conversion rate at homepage is low as people are reluctant to register for new account. PanelPlace is growing its user base, therefore, this is the most critical issue in the website. The client wanted to take this opportunity to communicate with user about the rebranding and new features.

### Project Objectives

Redesign the homepage to encourage more people to register for new accounts.

### Success Measurement

A higher conversion rate at homepage, where people signup for new account.


## User-Centered Design 

I worked together with Esther Fan, user researcher in this project. 

### Objectives

In this first phase of this project, we want to understand people’s needs and goals when they see the homepage. Therefore, we have a better insight about users and from that, brainstorm ideas of solution. 

### Competitive Analysis

People like to search for different alternative before deciding which one to buy/use. We want to understand our competitor and therefore set our value proposition right so people can know which is unique about PanelPlace

My colleagues, Esther quickly did analysis of competitors in the local market and how the website help them achieve their objectives. The client also discussed with us on how different they want to be from other competitors. 

### User Interview

We want to understand what people think when they reach the homepage, and why they don’t register for new account. This phase is to understand their needs and goals at homepage

Novice and Expert User. In PanelPlace, the categorical criteria are:

- How the user know about paid survey before joining PanelPlace
- How well the user earn money in survey panel recommended by PanelPlace
- What is the goal of users signing up for PanelPlace?

We interviewed 6 users. The questions are structured to help us gain insights into their goals and needs in the platform. Some people join the platform just because they have free time and want to spend on earning some money. Others are very systematic about how to manage their earning and want to be efficient when doing survey. 

### Personas and User Journey

This is to produce representative of the user of PanelPlace so that we can tailor the content of homepage to this user

After interviews, we built personas that represent user of PanelPlace. A user journey was compiled with different pain point at different stage in using the platforms. We looked through user journey and list down all negative and positive experience at different stages in the platform. Some problems were common among interviewees, some were unique so we prioritised the list and started brain storming about solutions to these problems.

### Collaboration Workshop with Stakeholder

The early involvement of stake holder in wireframing is important to a faster approval of design later since stockholder will have a better sense of ownership in design process. 

This project is the first time we experiment collaboration workshop with stakeholders. We wanted clients and designers to be aligned with each others about what the design will look like. 

<figure>
  <img src="/images/panelplace/collaboration-wireframe.jpg" alt="">
  <figcaption>Screenshot of different idea/sketch all together</figcaption>
</figure>

## Design Measurement

### Objectives

At the time we was working on wireframe of the new homepage, we talked about how to validate design. This topic lies in a gray area of design. The approval of design was mostly done by stakeholders, which explain the subjectivity and why some design though approved was not successful after launch. We wanted to use data to assist decision making in choosing best design


### Research

Since I had been working with Google Analytics, I did the research on A/B Testing and other usability testings. I presented to my team first and then client about this usability testing methodology. Everybody feel excited about this testing method and decided to adopt this in the project.

I discussed with our client, Denniz about the important metrics to measure in the homepage. As the objective of homepage is to increase more new new account registration, the key metrics of the homepage is the conversion rate measured by how many percentage people click the signup buttons in in the form located at a few places in homepage. 

We started with a multivariate test for different changes at the signup form. Among all elements in the homepage, signup redesign have the most impact on changing the conversion rate.

At the time, I was following Good UI and subscribing to their newsletter. As they recommended Visual Web Optimizer (VWO), I decided to use try it out. Google Analytics require a longer time to set up while Optimizely turned me off when it required credit card for trial. I liked the interface and how easy it is to setup a test in VWO.

### Tryout

When I started the 1st test in the project, I was anxious about the progress of the test and aways hope to get a early winner. I kept checking the result frequently in a day and felt happy whenever there is a winner. However, it turned out that the more people went to the homepage, the more accurate the result is and for most of the time it gave me surprise.

Due to the traffic side of the website, I had to wait for many days before having a winner. However due to the slight improvement, it is really hard to reach a high confidence level (95%) as we reach maximum 92% after 7 days testing. As this is our first, we still accept this result and proceed with implementing the new headline. 

We noticed that with small change like the headline, the improvement is very also small and the confidence level takes time to get to 95%, which is considered as standard in A/B Testing. 

### Signup Form Test

**Objective**

We want to know if simplifying the form, adding more information of registration process will lead to better converion.

![Screenshots of Control and Variation]({{ site.url }}/images/panelplace/abtest-signup-form.jpg)

**Control**

![Screenshots of Control]({{ site.url }}/images/panelplace/abtest-signup-form-control.jpg)

This is the original signup form in homepage, with its position on the right. The section Why PanelPlace is a informative part that is put under the signup form. The social media signup is not needed. We used heatmap to monitor the homepage and found out that people rarely use this functionality.

**Variation**

![Screenshots of Variation]({{ site.url }}/images/panelplace/abtest-signup-form-variation.jpg)

In this variation, we proposed a more informative signup form explaning different step in signing up to become member. The form is simplified to only 2 fields. The select box Country is important as it will decided the content user receive after signup. We want to make sure this is confirmed when people signup. 

**The Result**

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

#### Signup Button Test

**Objective**

After this test, we want to improve the button since it is the most prominent element in signup form. In this test, we want to have more variations to test against the control. 

The 2nd test is the colour and text of sign up button. To solve the traffic issue, our client help put up more Adwords ads and boost up the traffic to the homepage. 

**Control and Variations**

![Screenshots of sign up button]({{ site.url }}/images/panelplace/abtest-signup-button.png)

**Result**

There are 1 control and 4 variations. I ran the test for 7 days. During 7 days, within the first 3 days, there are 2 variation lagging behind other variation so I decided to stop traffic going through those variation. In 5th day, anther variation lag far behind, it was stopped. The test now is about whether the last variation is more effective than the control. In this 2nd one, I got an relative improvement of 14.8% at 96% confidence level within 7 days.

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

Due to the time constraint of the project, I tested only a few important elements. Some copies and images were not tested. The traffic to the site is not enough for more A/B tests.

## Development 

After finding the best design, we implemented the new homepage on the live site. This was a quick job since the we already had HTML, CSS components from prototype of testing. 


## The Result

We increase the conversion rate of website for Singapore users. There is a slight decrease in other countries. *Data will be updated soon*. 

When the site is launched, the improvement is relatively smaller than result of tests. The reason, we agreed, is that conversion rate is decided by not just individual elements but as a whole with their complex relationship. Considering time and traffic constraint, the testings did help my team improve the design a lot, together with convincing client to implement the designs to live site. 

[PanelPlace.com with new design](http://www.panelplace.com)

## Lessons Learnt

**Data-driven design**

I know what worked, what didn't. All were proven by data from real users.

**Working together with stake holder**

I love working directly with stakeholders. The message is delivered across the table without any loss in translation. In this project, I worked with Denniz, co-founder of PanelPlace. We discussed a lot during multivariate testing phase. That’s why we managed to have a considerable traffic to the site during testing and therefore, lead to successful result. 

**Ask better question**

During this interview phase, we also learnt that the question is not about having more conversion at the homepage but it’s about delivering the promises. When designing homepage, we see that a better conversion rate at homepage doesn’t necessarily lead to more long-time users. Having an attractive copy in homepage is like giving a promise. Whether or not we can deliver what we promise is also important. That’s why we in the homepage, we try to write a copy that is close to what the platform can do for users. 

<hr/>
This case study is published with permission from [Denniz Kee](http://sg.linkedin.com/pub/denniz-kee/28/34b/a), founder of PanelPlace
