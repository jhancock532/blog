---
title: Development Considerations
project: Network Practices
date: 2021-02-02T14:42:39+00:00
author: James
layout: post
permalink: /website-development-considerations/
tags:
  - Reflective Writing
  - Web Projects
---

This website will require the dynamic loading and instancing of several character models, alongside animation mixing management. My previous Three.js coding layout of "putting everything in one file" will not be suitable for this project, so it's time to create a custom class file.

I am creating a Participant class which will handle the loading, modification and mixing of all the participant models. Using a game engine would be the easy solution to this problem, but I recognise a good opportunity to learn more about JavaScript and async and await. 

![Lighting and Shadows](/blog/assets/images/lighting.jpg)
*Lighting and shadows working well, might remove shadows if more than six models are in the scene.*

Having messed around with this a bit, I've realised that concurrency isn't a big deal for this website, as the models are rather small. I've set up the code so that I can have a loading screen appear while the participant is waiting in the future. I'd like to load the site models concurrently, but this is an addition for further development. Currently my code is fingerprinting the browser and loading models at the same time, then checking to see if both these processes are finished in its animation loop.

The models are loading into the site with their material styling dependant on the fingerprint hash of the browser. There were a few tricks with cloning materials / cloning animation skeletons required to make it work, but now I have any number of models that can be loaded in each with an independant animation mixer, all managed by Participant.js.

![Models waiting patiently to be animated across the internet.](/blog/assets/images/patience.jpg)
