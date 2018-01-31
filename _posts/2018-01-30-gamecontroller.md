---
title: Game Controller
subtitle:
date: 2018-01-30
author: Lin Zhang
layout: post
comments: true
category: tangbileInteraction
---

For the first assignment game controller with HID output, I chose to make a controller for this version of the [Lunar Lander](http://moonlander.seb.ly) game:

![lunar lander]({{ site.baseurl }}/img/tangible/lunarlander.png)

To play this version, the users have to press the up, left and right key, and the mouse.

For my design, I implemented a controller that is a combination of sensor and buttons. More specifically, [Adafruit BNO055](https://learn.adafruit.com/adafruit-bno055-absolute-orientation-sensor/overview) absolute orientation sensor to control the direction. Two buttons, one button for mouse click and one for the up key.




<iframe width="1280" height="720" src="https://www.youtube.com/embed/qDT6c9QYbU0?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
