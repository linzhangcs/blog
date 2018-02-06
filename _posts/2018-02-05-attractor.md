---
title: Attractor
subtitle:
date: 2018-02-05
author: Lin Zhang
layout: post
comments: true
category: natureofcode
---

For week two, I want to explore attractor force and see what kind of pattern I can generate with it.

After following the lecture on attractor on Kadenze, I have a basic sketch of attractor and particle simulation.

![attractor]({{ site.baseurl }}/img/noc/basicattractor.png)

Since I have attractor and particle class, I experimented with adding more particles and attractors to the canvas.

![attractors]({{ site.baseurl }}/img/noc/multiattractor.png)

As shown above, when it's only drawing particles as points, the direction of the particles are not being represented. To do that, I added history array for particle class. Also I experimented with the initial conditions of the particles - position, mass, velocity. Here are some captures of the ones that are more dynamic.

![attractors]({{ site.baseurl }}/img/noc/movement.png)

![attractors]({{ site.baseurl }}/img/noc/movement2.png)

![attractors]({{ site.baseurl }}/img/noc/movement4.png)

![attractors]({{ site.baseurl }}/img/noc/movement5.png)

Project code can be found [here](http://alpha.editor.p5js.org/linzhang/sketches/HJRc8NDUM)
