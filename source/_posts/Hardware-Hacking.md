title: "Hardware Hacking"
date: 2014-11-13 18:08:53
tags:
- Tessel
- hardware
- PubNub
---

his month I attended a hardware hackathon. I haven't done much hardware past computer and organization design class. The hackathon was about two technologies, Tessel and PubNub. Tessels are small computers on integrate circuit chips (micro controllers). PubNub is a data streaming network that lets you send data through channels that devices can subscribe to.


The cool part about this hackathon was that it was easy to work on this together since there were two separate parts that came together. My team created a self measuring ball for a physics class. A ball that would measure it's own trajectory when thrown instead of video taping the ball's movement and working out the trajectory from there.

In order to do that, we used JavaScript to communicate with the Tessel, which was wrapped in paper towel to mimic a ball. That data was then sent to PubNub, and then translated to a graph of the x and y coordinates using Python.

Our team ended up winning first prize, which was pretty awesome. We all received free Tessels. It was great to get an opportunity to work with hardware, and I would definitely do it again. You can check out the project on [github](https://projects.tessel.io/projects/tessel-toss)

Action Items

* Learn how to update automatically with information from Tessel aka use the callback function in real time
* Learn D3 or Matplot lib for an animated graph
* Do something cool with my Tessel
