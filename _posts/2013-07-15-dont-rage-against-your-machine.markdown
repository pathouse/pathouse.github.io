---
layout: post
title: Don't Rage Against Your Machine
date: 2013-07-15  5:25:52
categories: tldr front
tags: programming web developer web development ruby on rails code coding testing javascript learning
---

What did I do this week? I wrote tests. So now we know two things. First, I wrote tests (well I learned a new testing framework and then I wrote tests, technically, and the learning took much more time than the writing, but I digress). Where was I? Ah yes. First, I wrote **Tests**. Second, I work for a company called **Artsicle**. Put two and two together, mix it in with my penchant for clever titles, and you have a recipe for a gleefully immature punstravaganza. It was so hard for me not to indulge this whim. Thank you for appreciating my will power.

### A Whole New World
When you're working with a testing framework called **Jasmine** and you've seen Aladdin as many times as I have (many times), it's hard not to make that your first header, and the header of the page on the company wiki, and many other things beside.

Alright, enough with the tangents. Onward and upward. Yes, so, I learned, through many trials and many errors, how to get [Jasmine](https://github.com/pivotal/jasmine "") up and running and working with our Rails app. Though, it's never really quite as simple as a single framework, as young neophyte programmers like myself quickly learn. What I ended up putting into place was a combination of the [Jasmine-Rails Gem](https://github.com/searls/jasmine-rails "") and three helper JavaScript files:

* [Jasmine-Fixture](https://github.com/searls/jasmine-fixture "")
* [Jasmine-jQuery](https://github.com/velesin/jasmine-jquery "")
* [Jasmine-Ajax](https://github.com/pivotal/jasmine-ajax "")

Each of which extends Jasmine's capabilities in some way. They should all be obvious except maybe Jasmine Fixtures, so I'll just tell you right now - it lets you programmatically append elements to the DOM within your tests so you don't have to write separate HTML files.

Jasmine tests JavaScript. Testing in general is a pain because of all of the necessary "environment simulation" or whatever you want to call it, but testing JavaScript is extremely painful. **Pain and gain, baby. Pain. And. Gain.**

### Baby Don't Hurt Me, Don't Hurt Me, No More
There were many frustrating things about learning this framework. Right off the bat, I initially found one gem that was easy to set up and seemed to work like a charm, but it was no longer being supported. It was a little orphan that had been abandoned and despite having twice the number of downloads as the next most popular gem (the one I ended up using) it was no longer under active development and that's not good in the fast-paced world of web development. If you're not on the bleeding edge, you're just slowly bleeding out. Maybe if I wasn't brand spanking new at all this and if it wasn't taking all of my energy just to keep my head above water, I would have taken it under my wing, but there's no looking back now.

So it took me a long time to figure out how to get this new framework put together and I was still angry I had to abandon the much easier one, so naturally I just had bad feelings toward anything new or different that I was forced to adjust to. Blah. Don't do that. Don't be angry at things that are new and different. That's not helpful. Also, having learned it all, I realize that the way I ended up doing things is much better and smarter in the long run. Easy is not a synonym for good, no matter what that bootleg thesaurus you picked up in the dollar store around the corner says.

### Pioneer Fear
I was the first person on my team to learn this framework and get it working. So if you don't already know this, all those guys on Christopher Columbus' ships weren't having the time of their lives. Being the first to do something is not all fun and games. Now, before I get all carried away and dramatic here, no my friends and family didn't all die of snake bites and dysentery (Oregon trail, Columbus, mixing metaphors, deal with it). But for the first time there was no one on my team with previous experience I could ask for help. Yeah, the Internet, I know, I eventually learned it. I guess what I'm trying to say here is that there are a number of times I can look back and safely say that I was feeling overwhelmed and angry that things weren't easier. Blah. What a bunch of nonsense. Sometimes it feels like I keep learning the same lesson over and over again, but at least I'm learning.

### What's the Lesson? Did He Say What the Lesson Was? WHAT'S THE GODFORSAKEN LESSON!?!?!
I'm tired so you're getting a list of rules that summarize what I have had to learn time and time and time (repeat ad nauseum) again over the past 6 weeks. And I'm going to shout them at you because I want to go back into the past and shout them at myself and I can't do that so I'm shouting through you vicariously.

1. **DON'T PANIC**
2. **BE PATIENT**
3. **FAILURE HAPPENS. IT'S NOT PERMANENT**
4. **ONCE AGAIN, STOP WORRYING ABOUT FALLING DOWN AND JUST DO IT, YOUR FACE WILL BE FINE, IT'S ONLY A METAPHORICAL FALL**
5. **THINGS WORTH DOING TAKE TIME AND EFFORT**
6. **ROME WASN'T BUILT IN A DAY. SHUT UP, I KNOW IT'S A CLECHE. ROME WASN'T BUILT IN A DAY, ROME WASN'T BUILT IN A DAY. ROME WASN'T BUILT IN A DAY.**
7. **STOP EXPECTING TO UNDERSTAND EVERYTHING THE FIRST TIME YOU READ IT.**
8. **FRUSTRATION IMPEDES LEARNING. DO NOT GET FRUSTRATED, GET DETERMINED. THIS IS A LONG DISTANCE RACE, ENDURANCE TRUMPS SPEED.**

Originally posted on [Tumblr](http://patmcintern.tumblr.com/post/55489205964/dont-rage-against-your-machine)
