---
title: Cutting Grass
project: Network Practices
date: 2021-02-02T14:42:39+00:00
author: James
layout: post
permalink: /cutting-grass/
tags:
  - Reflective Writing
  - Web Projects
---

I'm using the image of a fingerprint to determine where my grass is grown.

My image was originally too large, meaning my algorithm for finding the next empty space to add a grass model was running very slowly. I have reduced the size of the image and now it runs faster.

It would be better to scan through the image line by line I think and add instances of the mesh this way - I will have to adapt the random placement code even further for this, a good way to learn more javascript.

Instances of the grass mesh load and run incredibly fast, 144fps without any stutters and I've got 3000 times 100 polygons in play. 

I recently discovered the fingermaze in Hove Park, Brighton. It's a traditional labyrinth elongated to become a fingerprint with extra paths added for more fingerprint height. I have drawn a replica of the pattern as a layout for the grass in my garden.

The pattern looks pretty boring. It's just a standard seven ring labyrinth with some peusdo rings added to the top of it. I've left it in my code, hidden behind a variable change, but I'm going to stick with my first design.

Adding flowers to the scene; I'm using a similar strategy as the character model loading, except I've preprocessed the flowers in Blender so that I can import 12 different flower designs in one glb file. This saves a few HTTPS requests - my code then seperates out the objects from the file.

The flowers are scattered randomly throughout the fingerprint. My code uses flower positions it identified whilst finding valid positions for the grass of the fingerprint, so the flowers are placed nicely within and nearby the grass instances.
