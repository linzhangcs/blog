---
title: Exploration of narrative in 3D
subtitle:
date: 2018-10-03
author: Lin Zhang
layout: post
comments: true
image:
tags: [Computational Approaches to Narrative]
---

During the course of this class, we explored with a lot of tools and programs to generate text based narratives. In those narratives, we discover objects and space through text based description. I find that process very interesting and challenging. It is interesting because I can imagine the specifics, but challenging because it becomes difficult to keep track all of the connections in my mind. I found myself gravitate towards more visually represented tools, like ren'py because of that reason. Originally, I proposed to adapt a story I did in twine in ren'py. However, I looked more into more ways to produce a visual story. I wanted to explore narrative structure in Unity.

Unity is great for creating a 3d environment, but there is not a way to give narrative structure to all the interaction. I wanted to know if there are existing ways to integrate them.

My exploration started with trying to integrate twine stories into Unity. I found a plugin called [Cradle](https://github.com/daterre/Cradle), added it into Unity. Also, played a cradle game called [snoozing](http://daterre.com/projects/snoozing/). I found out it converts an existing twine story into Unity objects in a scene, rather than parsing the branching narrative logic in a twine story. I was hoping to add AR components to interact with the story, however, using Cradle would not be the best choice for it.

Here is a video of Cradle in Unity:

<iframe width="560" height="315" src="https://www.youtube.com/embed/AQKOWikDlJ0?start=3" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

I spent more time looking into tools that would enable me to add story logic to Unity. I came cross a plugin called [Fungus](http://fungusgames.com/). The creator introduced it as being inspired by Twine and ren'py.

Also, I played one of the games that is made with Fungus, called [Lieve Oma](https://vltmn.itch.io/lieve-oma).
![granny]({{site.baseurl}}/images/narrative/lieveoma.png)

![fungus]({{site.baseurl}}/images/narrative/fungus.png)



Fungus is what I was looking for adding story logic into unity. Once fungus is installed and imported, it offers a flowchart for the game logic and keeping track of variables. It is very simple to use and works well with Unity existing uses of the program UI.

![flowchart]({{site.baseurl}}/images/narrative/flowchart.png)

With the time I have, I only implemented a scene of the storyline. It is the boy founding a dragon in his room.

![boydragon]({{site.baseurl}}/images/narrative/boydragon.png)
