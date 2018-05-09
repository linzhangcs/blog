---
title: Googlemancy & Prayer Device
subtitle:
date: 2018-05-08
author: Lin Zhang
layout: post
comments: true
category: electronicrituals
---

For my final project, I want to continue my "-omancy" divination invention, Googlemancy. It was inspired by Google's "I'm feeling lucky" option. To improve the project, I want to add the following features:

- Give users instruction and context for the ritual
- Create something out the search result - a visualization or poem
- Add wearable device to enhance the physical aspect of a religious ritual

I found a website devoted to Google as a religion - [Church of Google](http://churchofgoogle.org/). Using their prayer section, I got some very profound message to use as copy to establish context for the visitors.

As users following the steps of the instruction, they will input their question, date of birth, and asked to bow down 3 times to send a request to Google.

![intro text]({{site.baseurl}}/img/electricRitual/intro.png)

![3rd step]({{site.baseurl}}/img/electricRitual/3rdstep.png)

The result is a poem composed based on the text from the selected website.
![result]({site.baseurl}}/img/electricRitual/result.png)

![result]({site.baseurl}}/img/electricRitual/languageParts.png)

I used Google custom search API to search based on the question, and select the website using the users' date of birth. Once a website is selected, I send out another request to retrieve its page as a html string. After parsing the html string, I used [compromise.js](http://compromise.cool/) to parse all of the nouns, verbs, and adjectives to create a poem using a pre-defined sentence structure.

Here is the accompanying wearable for this project:

![device]({{site.baseurl}}/img/electricRitual/wearablefront.JPG)

![device]({{site.baseurl}}/img/electricRitual/wearableside.JPG)

![device]({{site.baseurl}}/img/electricRitual/wearableback.JPG)

![device]({{site.baseurl}}/img/electricRitual/circuit.JPG)

![device]({{site.baseurl}}/img/electricRitual/prototypes.JPG)

![device]({{site.baseurl}}/img/electricRitual/finish.png)

Here is a video for testing & presentation

<iframe width="860" height="415" src="https://www.youtube.com/embed/jva6e_tqXy8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


<iframe src="https://docs.google.com/presentation/d/1iDZwyBPAMfFQUwBR4FGGC2nSOhLT5dDw-tnlaJPxcyw" width="1000px" height="500px"></iframe>

Lastly, here is my [code repo](https://github.com/linzhangcs/googlemancy/). You can try the website [here](https://linzhangcs.github.io/googlemancy/)
