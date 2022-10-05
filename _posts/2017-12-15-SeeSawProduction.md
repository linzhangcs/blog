---
title: SeeSaw production
subtitle:
date: 2017-12-15
author: Lin Zhang
layout: post
comments: true
categories: PhysicalComputing
image: pcomp/IMG_5163.JPG
tags: [Physical Computing]
---

### Seesaww Design Process

#### Scenario

![scenairo]({{ site.baseurl }}/assets/img/posts/scenairo.jpg)

#### User Flow

![user flow]({{ site.baseurl }}/assets/img/posts/userflow.jpg)

#### Play Testing

Before we build a full scale seesaw, we tested the project concept by conducting a play testing session of 30 users. My partner and I recorded and collected the user experience and feedback. The initial prototype utilizes items we had in the shop and used them as a representation of our project components and features. For example, the seesaw was represented by a broken workout bench and a small ladder. The LED lights on the sides of the bench are supposed to be LED strips.

![prototype]({{ site.baseurl }}/assets/img/posts/prototype.JPG)

![feedback]({{ site.baseurl }}/assets/img/posts/feedback1.png)

<iframe width="560" height="315" src="https://www.youtube.com/embed/JFiLjI0zXUg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

Based on the feedback, we removed the lighting feature and came up with strategies to start the game.


### Fabrication

*Why build a seesaw? Can't we buy one?*

The intended audience is adults. We searched for seesaw for adults with no results on the major online retailers: Amazon, Aliexpress, and Google shopping. The ones we can find are designed for kids from age 4 to 8. To ensure a safe and fun experience, we built a seesaw that is measured and designed according to the body size of adults.

#### Bill of material

![BOM]({{ site.baseurl }}/assets/img/posts/bom.png)

Items with grey background are materials we planned but did not use. The ones with yellow background are those we did not plan but used in our project.

#### Seesaw Design

![seesaw design]({{ site.baseurl }}/assets/img/posts/design.jpg)

#### Fabrication Process

![fab]({{ site.baseurl }}/assets/img/posts/fab.jpg)

![fab]({{ site.baseurl }}/assets/img/posts/fabp.jpg)


### Physical Computing

#### Circuit Diagram

![circuit]({{ site.baseurl }}/assets/img/posts/circuit.jpeg)

We used the following sensors :

* [Adafruit BNO055 Absolute Orientation Sensor](https://learn.adafruit.com/adafruit-bno055-absolute-orientation-sensor/overview)
* [Pressure-Sensitive Conductive Sheet](https://www.adafruit.com/product/1361)

#### Sensors testing

![pressure sensor]({{ site.baseurl }}/assets/img/posts/pressuresensor.jpg)

![BNO sensor]({{ site.baseurl }}/assets/img/posts/bno5500.jpg)

#### Serial Communicaton

<script src="https://gist.github.com/linzhangcs/623ccec9589cc2475bb674f2a97986b3.js"></script>

### Brick Breaker - Game Component

Under the time constraint, we decided to build on an existing game. Our code is based on this [brick breaker github repo](https://github.com/James-Hynes/Breakout). We polished the game interface and add needed features to integrate it into our project.

#### Interface Design

![game interface]({{ site.baseurl }}/assets/img/posts/gameInterface.jpeg)

#### Game Features
From the the play testing feedback, we added features for a more enjoyable experience:

* Serial Events - get data from pressure sensor and orientation sensor
* Countdown timer
* Game reset - redirect back to splash screen once a game ends
* Interface update - color, font, layout
* Splash screen

### User Testing

<iframe width="560" height="315" src="https://www.youtube.com/embed/1-hPAmv1omY?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

#### Feedback

![feedback]({{ site.baseurl }}/assets/img/posts/feedback2.png)

### Final Product

![seesaw final]({{ site.baseurl }}/assets/img/posts/seesawfinal.jpg)

![seesaw final]({{ site.baseurl }}/assets/img/posts/seesawplay.jpg)

### User Testing - Part Two

<iframe width="560" height="315" src="https://www.youtube.com/embed/8IrklmpCEk0?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>