---
title: Chequered Waves - Bees & Bombs
subtitle:
date: 2018-02-11
author: Lin Zhang
layout: post
comments: true
categories: natureofcode
image: noc/cqtwocolors.png
tags: [Nature of Code]
---

I decided to create one of [Bees & Bombs](https://beesandbombs.tumblr.com/)'s gifs for week 3. I selected this gif:

![chequered waves]({{site.baseurl}}/images/noc/chequeredwaves.gif)
***Chequered Waves***

<!-- ![sea urchin]({{site.baseurl}}/images/noc/seaurchin.gif)
***Sea Urchin*** -->

For the Chequered Waves, I followed one of Dan's [coding challenge](https://www.youtube.com/watch?v=H81Tdrmz2LA) videos as a starting point. The behaviors of the two are very similar.

This is what I have after following the video, the visual is off.

![lol](https://media.giphy.com/media/xThta2R12AHTZ3DNM4/giphy.gif)

After looking over the code again, I discovered the bug is one of the offset variables is being updated in the wrong place.

![updown](https://media.giphy.com/media/d3YI5l21Aiet66iI/giphy.gif)

Once I recreated the example, I realized instead of using changes in height, I need to translate the positioning of the boxes along the Y axis. But first of all, I need to generated the boxes in chequered pattern:

![cp]({{site.baseurl}}/images/noc/cp.png)

![cqtwocolors]({{site.baseurl}}/images/noc/cqtwocolors.png)
**_For some reasons, (0, 0) seems to be at (width/2, height/2). What do I set to start at (0, 0)? I have so many questions._**

I did not have experience with WebGL or OpenGL, so the 3D environment setup is very new to me. I wanted to have an idea how to setup camera, perspective, lighting, and material in 3d, I watched Dan's playlist on [WebGl in p5.js](https://www.youtube.com/watch?v=nqiKWXUX-o8&list=PLRqwX-V7Uu6bPhi8sS1hHJ77n3zRO9FR_) and followed along. To focus more on last week's topic, I decided to leave the camera rotation part for later, and just work on the oscillating movement for now.

Once I have the pattern with boxes, I just to need to translate the change along Y axis. I experimented on how to generate offset for a while. Here are some of the variations:

![2waves](https://media.giphy.com/media/1JKvv6q0eWJHpq2XL6/giphy.gif)
***The edge boxes are too far apart***

![lowres](https://media.giphy.com/media/THDh9LtRZHcH7alafn/giphy.gif)
***Improved the edge, noticed overlapping***

![final](https://media.giphy.com/media/28GQguS8qnN71ZaKSd/giphy.gif)
***What I have so far***

Also realized my current way of recreating the original gif is not the best way. This implementation can't use 9*9 grid to produce desired oscillating movement, because 9*9 is not enough to visually present the overall motion. Maybe, I can use the Chequered image as a texture. It can be mapped with points that textual moves on. I did not find any texture UV coordinates related function in p5.js. After doing this exercise, I feel like I learned some basic usage of WebGL in p5.js.

Project code can be found [here](http://alpha.editor.p5js.org/linzhang/sketches/HyQ0nmgvf)
