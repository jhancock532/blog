---
title: Moving and Sitting
project: Network Practices
date: 2021-02-02T14:42:39+00:00
author: James
layout: post
permalink: /moving-and-sitting/
tags:
  - Reflective Writing
  - Web Projects
---

I've added an extra pub-sub message for when a character model moves to a new location. I am now very tempted to add real time sitting down on the garden benches. After this is developed, then the focus is on the user interface - tooltips that appear when you mouse over other participants, to learn if they are a ghost / real and to identify who you are. A nicer loading sequence and introduction to the website would be great as well.

Time to create a new Bench class... or perhaps think about the logistics and how I'm going to implement this over pub / sub. "Sitting On Bench" is going to be another character attribute that gets sent in the pub sub message, it should be an integer - sitting on bench id 0, 1, 2, 3, or if not sitting, null.

Walking to the correct position is already done - the animation of turning around and sitting down is perhaps a good goal to work towards. The bench class will need to have it's angle publicly accessible. What if two people can sit on a bench? Bench ids 0 and 1 both refer to seats on the first bench? Well, the bench model itself can be ignored really, we can use invisible "sittable" cubes that just so happen to overlap where the benches are.

Implementation of the initial bench positions and sitting down animations has gone smoothly, bar the totally wild rotation movements. I'll have to slerp quarternions to get the rotations to always go the easiest way, but that's not an essential requirement. Now it's time to hook up the client logic that tells others when a participant is sitting down - it would be nice if that seat is then reserved for that participant. If the seat isn't free, but the seat beside it is, then the participant should automatically move to take that seat instead.

The sittable cubes sadly overlap each other - I will add logic to my raytracing that the last cube the ray hits is the intended cube, as the user can't see the cubes and often clicks through them. Also, I'm pretty proud of how you can now see characters walking across the screen on multiple devices, with positions synced correctly - now to implement the same process for the sitting movements. But first, some lunch.