---
title: Changing faces - projection mapping
subtitle:
date: 2018-09-19
author: Lin Zhang
layout: post
comments: true
image: magicWindows/test-projection.JPG
tags: [Magic Windows]
---

I partnered with Mengzhen for this project.

Initially we wanted to project markup to users' face and they can switch to different set of markup looks.
We did a quick test run for this idea. We found out the projection on the face is too bright for the idea to work.

![markup image]({{site.baseurl}}/images/magicWindows/p1.png)

![markup test]({{site.baseurl}}/images/magicWindows/markup.JPG)

After that test run, we decided to project a face onto our face to create a new look. Mengzhen picked Taylor Swift and we projected her face on our face. Here is the results:

![projection]({{site.baseurl}}/images/magicWindows/test-projection.JPG)

![projection setup]({{site.baseurl}}/images/magicWindows/setup.JPG)

![Mengzhen Swift]({{site.baseurl}}/images/magicWindows/test-face-two.JPG)

![Lin Swift]({{site.baseurl}}/images/magicWindows/test-face.JPG)

After testing out Taylor's face, we wanted to try out a collection of faces and using our voice as user input.

The tech stack we used is
1. Processing
2. Keystone
3. Web sockets - [webkitSpeechRecognition](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

Here are the videos
<iframe src="https://www.youtube.com/embed/Czpe1D-LkcE" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


<iframe src="https://www.youtube.com/embed/QWDML2B-2tc" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
