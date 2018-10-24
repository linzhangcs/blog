---
title: ML Image Recognition in AR
subtitle:
date: 2018-10-24
author: Lin Zhang
layout: post
comments: true
image: magicWindows/mlar.png
tags: [Magic Windows]
---

For midterm project, My partner, [Mengzhen](https://www.mengzhenxiao.com), and I want to explore machine learning image recognition in AR.


## Concept

So far in class we explored using image or object targets for adding augmentable into the space. While it is a great way to trigger changes, we want to see an experience that would react to objects without the constraint of selecting and adding a target first.

Mengzhen has experimented with an example of AR experience that would recognize a drawing of a clock and shows a working digital clock to the user.

<iframe src="https://www.youtube.com/embed/hoRNVjwJf0w" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

We found the direct translation from real life to digital representation as an area that is rich exploration. Especially, if the application would recognize and react to the objects in the physical environment.

<iframe src="https://www.youtube.com/embed/PIJc0TSDdRo" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

Once the object is recognized, there are multiple ways of react to it in AR experience:

- **Create new augmentable in the scene**

  ![ar clock](https://media.giphy.com/media/EczciuU6VuEoGXxITY/giphy.gif)
-  **Add special effects to the physical object**

  ![effects](https://www.thisiscolossal.com/wp-content/uploads/2014/04/letters.gif)  

  ![effects](https://www.thisiscolossal.com/wp-content/uploads/2014/04/pensmoke.gif)  

- **Use the object abstractly - passed its name to 3rd party api or fetch related data**  

  ![tweetAR](https://media.giphy.com/media/fH92WkWMHVNjaiUAUb/giphy.gif)

- **Interaction between augmentable and real person**
  * voice recognition / voice command
  * facial expression
  * react to the changes in the physical environment

<iframe src="https://www.youtube.com/embed/6CNNJYKGluc?start=49" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
**Voice command**  

<iframe src="https://www.youtube.com/embed/NhJydpMkpug?start=170" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
**Reaction to changes in the physical enviroment**  

## Tech Stack

[Tensorflow.js](https://js.tensorflow.org/)  

[ARCore](https://developers.google.com/ar/)

<iframe src="https://www.youtube.com/embed/uPPo4QNOZZo?start=2" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
