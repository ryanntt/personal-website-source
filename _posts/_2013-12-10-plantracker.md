---
title: PlanTracker - Mobile App Design
date: 2013-12-10 18:22:29 Z
categories:
- projects
layout: post
summary: This is the last project in my time pursuing bachelor degree. The documentation
  of this project is in progress
---

This is the last project in my time pursuing bachelor degree. *The documentation of this project is in progress.*

## Project Overview

## Motivation

After doing a research in app market in Singapore in mid 2012, I realised that there is shortage of financial management apps. The current apps have poor user experience with confusing functionality. Most of applications have either too many functions or complex functions, which them very hard to be used.

My friend, Salyonn Koh and I were both interested in designing and developing mobile application that help youngsters learn personal financial management. We decided to do this as our final year project. 

As Salyonn and I were not familiar with product development framework, researching on this is really tough. Fortunately, Salyonn was having internship in Apple Singapore so she learnt about interface design, Model-View-Control in MacOS application development. My internship was with R/GA Media Group, Singapore and my project is about a mobile web applications. Having these foundation, we were excited to kick start this project.

## Challenges
People want to use application not only as a tool to manage finance but also as a guide to learn how to mange personal finance in the best way. 

## Objectives
We wanted to create a application that serves as an educational and financial planning tool. Users are able to create plans and track their progress by setting a target amount within a fixed period of time. Graphic indicators will be provided to allow users to track the status and progress of the plan. The user experience and interaction will taken into consideration with high priority. 

## Process

In this project, my job scope is more of front-end developer than designer. Salyonn was the main designer.

At first we planned to develop as a native iOS app, but then moved to web app. The learning curve of Objective-C was very slow for us in the first 3 months and we wanted to focus on what we are strong at, which is web development. We wanted to to publish this as web app, then use PhoneGap to package and publish on App Store.

### Research
to be updated

### Design

In the design phase, we created wireframe and wireframe prototype in keynote to understand the flow of our application. 

After this, we refine the wireframe and created hi-fidelity design on top of the wireframe. Before this project, I was a Windows user and didn’t know anything about Mac. Using Keynote to create mockup and prototype in Mac was much faster than I thought.

### Development

The whole application was built on top of Query Mobile framework. We used HTML5 localStorage as client-side storage for the application. The whole database will be in JSON format. We did plan to have a online database but then couldn't do it due to busy schedule in final year. 

We used Agile framework to plan our work. Once every 2 weeks, we discussed the progress of project and create to-do list for the next 2 weeks. We often give the application to our friend to receive feedback on certain changes of interface, interaction, features.

### Testing

An overload test was conducted to assess the performance of database and AJAX code that populate data in DOM. Around 20 plans were created, edited, and deleted. The performance was observed to be fast and responsive. The graph that draw history of financial took long time to finish loading.

The application were tested on iPhone and Android phones to assess the performance on mobile web browsers. The loading speed was really slow. At some points, a average-spec Android phone seemed to freeze even with plan list and some simple transitions. The same observation was also reported on certain forum about the poor performance of jQuery Mobile. 

## Result

After our graduation from university (July 2013), the application was still under development with the lack of account management and online database. However, as Salyonn and I had different paths of career, we decided to close this project and treated this as a good experience working together in something we like before getting our first jobs.

[Try the app here](http://goo.gl/JgqXb) 



