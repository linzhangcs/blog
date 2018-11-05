---
title: Purring Cat 2.0
subtitle:
date: 2018-11-04
author: Lin Zhang
layout: post
comments: true
image: haptics/cat2.jpg
tags: [Haptics]
---

For the Haptics final, we as a group wanted to improve the cat purring simulator we made during the last class. To make the petting experience more realistic, we decided to only allow one-directional petting, because that is how cats prefer to be petted.

To achieve that we moved the two FSRs one after another, so to check the order in which they are triggered. Also we wanted to clean up the circuit by reduce the wires we are using. We used wire wrapper to do that.  
We were all amazed by the awesome power of the wire wrapper!  

![wire wrapping]({{site.baseurl}}/images/haptics/wirewrapper.JPG)
![wire wrapping]({{site.baseurl}}/images/haptics/wirewrapperheader.JPG)
![wire wrapping]({{site.baseurl}}/images/haptics/wrapperc.JPG)
![wire wrapping]({{site.baseurl}}/images/haptics/wrappern.jpg)

Here is the original mountain of wire:
![original wiring]({{site.baseurl}}/images/haptics/mess.jpg)
And the much simpler breadboard:
![wiring]({{site.baseurl}}/images/haptics/simple.jpg)

After we cleaned up the wires, we played with different vibration pattern. Also the placement of the vibration motors. To give the user a sense of direction, we made and added a tail to the cat's body as well:

![vibration motors]({{site.baseurl}}/images/haptics/pur.jpg)
![motors]({{site.baseurl}}/images/haptics/purring.JPG)

We experimented with embedding the motors into the cardboard. However, we noticed the vibration would be directed towards to bottom. We reverted back to placing them on top of the cardboard, and closer to each other. Once we have the purring effect working with the one-directional petting. We shared kitty 2.0 with other ITP students.  
![vibration motors]({{site.baseurl}}/images/haptics/kitty2.jpg)
![motors]({{site.baseurl}}/images/haptics/playtest.jpg)

Here is the code for the project:
<script src="https://gist.github.com/linzhangcs/ed87ef921f67aadb2e992ae7825c5b55.js"></script>
