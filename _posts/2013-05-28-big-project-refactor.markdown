--- 
layout: post
title: First Major Overhaul for Ruby Project
date: 2013-05-28 11:09:00
categories: projects front
tags: ruby project refactor
---

## The Long Hard Stupid Way

This comes as no surprise, but there are many parts of my project that are more complicated than they need to be. The goal of this project was to [learn by hacking][1] and that's exactly what I've done. 

After all, I'm a true believer that, when you're learning something for the first time, it's often best to do things [the long hard stupid way][3]. Sometimes learning what doesn't work is just as valuable as learning what does. 

Up to this point, the entire project was built without loading any libraries, but that's about to come to an end. Just yesterday I completed Jumpstart Lab's [EventManager][2] project and learned about two libraries that are relevant to my project - `CSV` and `ERB`. So, today the goal is to create a new branch and implement these tools, which should significantly simplify the code. 

[1]: http://www.circleround.net/brainfart/front/2013/05/23/to-learn-hack.html
[2]: http://tutorials.jumpstartlab.com/projects/eventmanager.html
[3]: http://dolectures.com/lectures/do-things-the-long-hard-stupid-way/
