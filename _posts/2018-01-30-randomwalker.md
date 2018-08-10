---
title: Random Walker
subtitle:
date: 2018-01-30
author: Lin Zhang
layout: post
comments: true
image: noc/levy.png
categories: natureofcode
tags: [Nature of Code]
---

To expand on random walker, I experimented with levy flight, perlin noise and probabilities. I thought it would be interesting to add a way to generate more walkers. So when the walker is choosing to move in a direction, a new walker will is added that is moving in the opposite direction.

The sketch can be found [here](http://alpha.editor.p5js.org/linzhang/sketches/BJdMEdTSz)

![levy]({{site.baseurl}}/images/noc/levy.png)
![perlin]({{site.baseurl}}/images/noc/perlin.png)
![finalsize]({{site.baseurl}}/images/noc/finalsize.png)
![final]({{site.baseurl}}/images/noc/final.png)

After experimenting with different ways to create randomness, I find it hard to generate compelling images based on randomness alone. I think the walker needs to have some directives to follow or there has to be an underlining pattern as a structure to build upon.
