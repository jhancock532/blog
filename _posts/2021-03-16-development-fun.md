---
title: Development Fun
project: Network Practices
date: 2021-02-02T14:42:39+00:00
author: James
layout: post
permalink: /development-fun/
tags:
  - Reflective Writing
  - Web Projects
---

## Notes Made Whilst Debugging Network Connectivity

Attempted to set up a listener for websocket connection ending on the server side, however no easy way of connecting client id to client hash?

On connection event send client a message with client id? No way of sending a message like this. :(

Solution: after a client disconnects, send a message saying a client has disconnected. Then delete a random client?

Solution: 
client connects. 
Message is sent out from the server side with client id to active clients.
client has subscribed to messaging channel - first message it recieves is its client id.

RT database is updated with hash & client ID?

If a new client has joined, check the RT database.
If a new client has disconnected, check the RT database?

Although this is ineffiecent, I can just have the clients publish their existence in the group chat every so often.
I have free unlimited pub / sub messages so I can just reset a "time to live" timer for each participant.

265B36C8-4521-CF24-DEC8-4348F03FB238

participant presence is now entirely dependant on the server, as even the users participant is only kept alive if a pub / sub message is pinged back and forth from the server.

This has some historical precendent, IRC chat with ping / pong messages, polling, etc. TimeToLive isn't like actual network packet TTL but it works well.

## TODO

Put most of the Backendless code into a seperate file? Refactor?

Loading and selecting ghost participants to display from the server
Ghost participants should fade in and out on a loop, they should have different TTL and update rules.
Display a random ghost every 30 seconds, have the ghost creation and destruction overlap each other...
... ghosts shouldn't be shared across the server? What if the server pings a ghost message, once every 30 seconds?
Total number of ghosts should reduce as more people join; if only one person joins, there should be at least three ghosts to interact with.
Ghosts should be handled by the participant manager.

Showing the ghost participant age on hover (use a DOM overlay)


A "loading" screen that displays the participants fingerprint for a few seconds, whilst other models are loaded in the background.

A smart way of loading participants so they don't load into each other? Just use randomness, this doesn't matter too much if there is enough space. Select three positions randomly, use an algorithm to detect which is the best? I'm sure there is an algorithm for finding the best space to place a new node, like voronoi.


A detector for mobile devices that changes the quality of material used by participant manager & removes shadows.


On click raycasting that fetches the (x, z) position for the model to walk to

An animation cycle / model tweening of the model turning and walking to that direction, Tween.js


## Done

Updated lighting, only save hash to database if it is unique.

Refactor TTL so that is uses milliseconds.

Added basic ghost management, investigated how difficult fading in ghosts was - doesn't seem worth the computational effort to me.

After adding the ghost, I realised that adding shadows was a bit unnecessary for them.
![A ghostly friend](/blog/assets/images/aghostlyfriend.jpg)

Ghosts popping in and out is rather disconcerting. I have added Tween.js and I have successfully got them to disappear by animating their opacity, now trying to do the same for when they load in...

Success! Ghosts are fading in and out. Spooky.

Adding the DOM hover overlay... actually first, I'm taking a break.

Oh dear, while I've been developing, my host has gone down. RIP backendless

![A screenshot of a dead server](/blog/assets/images/notgood.jpg)

I take this as a sign that I should work on another project now.


https://en.wikipedia.org/wiki/Bricolage

In her book Life on the Screen (1995), Sherry Turkle discusses the concept of bricolage as it applies to problem solving in code projects and workspace productivity. She advocates the "bricoleur style" of programming as a valid and underexamined alternative to what she describes as the conventional structured "planner" approach. In this style of coding, the programmer works without an exhaustive preliminary specification, opting instead for a step-by-step growth and re-evaluation process. In her essay "Epistemological Pluralism", Turkle writes: "The bricoleur resembles the painter who stands back between brushstrokes, looks at the canvas, and only after this contemplation, decides what to do next."[20]