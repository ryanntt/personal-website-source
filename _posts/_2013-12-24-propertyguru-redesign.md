---
title: PropertyGuru
date: 2013-12-24 18:22:29 Z
categories:
- projects
layout: post
summary: This project is the first time I designed in HTML and last time used Photoshop
  in my workflow
text: Mobile web redesign
thumbnail: https://res.cloudinary.com/ryanntt/image/upload/s--WKdV-DQZ--/c_scale,w_768/v1506606844/propertyguru/thumbnail.jpg
  
---

This is the first time I designed in HTML and last time used Photoshop in my workflow.

## Project Background

During the first month after my last exam of bachelor degree (June 2013), I was applying for jobs and waiting for the graduation ceremony. I started improving my design skills through hackdesign.org, and when I learnt the lesson 10: Rapid Prototyping Tools & Best Practice, I found article [Fake it. Trash it. Build it](http://blog.42floors.com/fake-it-trash-it-build-it/). The article amazed me at the fact that any design workflow needs to be flexible enough to embrace changes and iteration, and that designer and developer need to work together in design process.

I became interested in creating design in HTML. Though the lesson is about tools, it is more about thinking process. I have been using Photoshop, Illustrator for creating design and agree that the process is dead slow, leading to frustration sometimes. 

I was looking for website or product interface to redesign using those skills I had just learnt. At the time, I was also looking for a place to rent so I tried several platforms such as PropertyGuru, STProperty, iProperty. Among these, Property Guru have more redesign opportunities for me. 

## The Challenge
There is a lack of focus in designing functionalities for mobile users. To search for property, user need to go through many steps. This is not helpful for users that need to search frequently.


## Design Objectives
- To improve the usability of search function
- To update the interface with a modern look


## The Process

-  Define business requirements
-  Finalise user stories
-  Wireframe
-  PSD and prototype in HTML

### Define Business Requirement
Since I used both website and mobile app, my first question was which platform should be redesigned. After checking Property Guru’s website and its mobile apps, I decided to redesign the mobile app since it is more challenging and the current design both on Android and iOS is quite poor.

I started by researching on Property Guru app and its business model. I found information about Property Guru Group’s history and some interesting facts in [this interesting article](https://sg.finance.yahoo.com/news/propertyguru-story-told-co-founder-051121686.html).

>“Steve (PropertyGuru founder) says that mobile is playing an increasing critical role for his company. Today 44 percent of PropertyGuru’s users are visiting from mobile devices, and this is expected to exceed 50 percent next year. ” 

This points did reaffirm my decision to go with mobile first.

After doing research online and asking my friends working in the realestate industry, I had following findings:

-  50% of the users are using mobile devices
-  Most users in Singapore are searching based on districts (location)
-  Price is the most used parameters, bed room is used by less than 10% of the users, size is the least.

### Build Feature List
This phase is quite hard to me since I have no background knowledge about property searching. After doing research on Property Guru, I realized an similar successful apps that I should look into: Airbnb. Though the business model of Airbnb and Property Guru are different, the interface that help people search for space to stay is quite similar so I thought I can look into good UX design of Airbnb to help improve PropertyGuru. I started using Airbnb and Property Guru app at the same time and compared them. During this time, I feel that designing a full experience from search to calling the owner/contacting agent is quite a big challenge. Therefore, I choose to focus on certain functionalities:

-  Users can search according to name of area
-  Users can use advanced search with price range, type of house/room, rent/buy
-  Users can see result page with enough information for user to decide
-  Users can see contact information of agent, and call agent

### Wireframe

All options were quickly sketched down in paper. The user flow is quite straight forward. Some questions are raised during this sketching phase:

-  What kind of information should be displayed in the result list and detail page of the item
-  What kind of advanced search setting we should have
-  How should the information of agent should be displayed in item’s detail page on mobile

After the first session of sketching, I improved on certain things:

-  The information in detail result page
-  Advanced search settings contains
-  Since contacting agent is the desired action of user after seeing favorite property, the CTA buttons should be displayed as an prominent part of the screen

I had been using Property Guru app for 2 days. I used the app in various situation: walking, in restaurant, on bus, before sleeping. I noted down what is the good and bad points of the app, and what functionality I would like to have. I did another round of sketching and then started working in Photoshop.

### PSD and HTML prototype

A first, I started with Photoshop. As the end product will be a mobile web so I tried to move to HTML prototype as quickly as possible.Together with creating HTML prototype, I work on refining the wireframe in Photoshop to become high-fidelity design.

![PSD Design]({{ site.url }}/images/propertyguru-redesign/propertyguru-redesign.png)

At that time, I read this amazing article [The Post-PSD Era](http://bradfrost.com/blog/post/the-post-psd-era/), by Brad Frost. 

I find that working in Photoshop has some constraints in flexibility. When I was creating wireframe, I looked into UI development of the prototype at the same time. One of the difficult part is how the side menu work. I researched on certain UI patterns for navigation and decided to go with side menu since it helps save screen space. Making this work in Javascript is quite challenging at first but also really fun. I prototyped certain UIs to test how the interaction work and therefore, I kept changing the Photoshop to reflect those changes. Seeing how slow working in Photoshop is, I completely moved to designing in HTML. I sketched down a few UI patterns and then tested how they worked in HTML. Together with interaction parts, I also tweaked colour and typography directly in HTML.


## The Result

I’m quite happy with the final result, [a prototype of redesigned PropertyGuru mobile web](http://goo.gl/ZioB9).

Following are my thoughts behind the visual design and prototype of this mini-project:

<strong>Visual Design</strong>

-  Since the main purpose of user is to search, the first page of mobile site is the most viewed listing, which is the result of blank keyword search with sort order "Viewed". The role of conventional homepage is reduced in mobile context.
-  The search bar can be toggled by pressing/clicking the icon on top right corner.Therefore, the user don't have to go to another page from the search result to start a new search.
-  Due to these 2 above reasons, my design has only 2 page: search result page and listing detail page. All are combined in single HTML file. 
-  The navigation menu can be accessed by pressing/clicking the icon on top left corner. This side menu helps save space so that users can focus on the main content and still can access menu quickly.
-  Font: Lato is used as it is clean, neat, especially when using with flat block of color.
-  The red in original Property Guru logo is pure red with high brightness and saturation, which make it hard to be included. -  Instead, a softer red color is used with more soothing looking in the design.
-  Besides new red color, different shades of grey are used to create clean looking. 
-  The limited use of color is due to the face that most adult user(especially male) consider colorful interface distracting.

<strong>Prototype</strong>

-  The prototype is not 100% responsive on tablet and desktop size since I only design for iPhone screen (I was still learning Foundation back then). 
-  There is no dynamic data injected into the html page as this is just a prototype. Dummy text is used, instead.

## Lessons learnt

<strong>Flexible workflow</strong>. After this mini project, I learnt that a static visual design serve little purpose in design process. Certain UI pattern are more familiar with designers now e.g. Side menu, toggle button ,search bar. The question is whether or not we can implement those UI in the product. I realized this clearly after implementing a few changes quickly in HTML.

<strong>Mobile first design philosophy</strong>. After designing the mobile site, I go to desktop site of Property Guru and felt overwhelmed by a  lot of funtionalities. It is hard, though, for a big site like PropertyGuru to go to mobile site since cutting down funtionality and content to fit mobile screen is a tough job.

## Update on 25 Jan 2015

I look at this mini project and want to revise a few things about mobile first design philosophy. After almost 2 year, I realised that people have higher expectation of what they can do on mobile. As a heavy mobile user, I can do most of the daily task I prevously did on laptop but on mobile phone now. From checking bank account, money transfer, paying bill, chat, social media, reading news, search and buy stuffs. So starting with mobile first is not easy at all, a mobile app with single purpose will have more functionalities soon, together with content added. It make us think about what is more important to have, what’s nice to have, which will stop us from adding unnecessary functionalities. In conclusion, designing on mobile first is still a good practice, but it’s getting harder and harder over time with higher expectation from users. 
