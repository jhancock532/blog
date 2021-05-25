---
title: Beta Release
project: Network Practices
date: 2021-02-02T14:42:39+00:00
author: James
layout: post
permalink: /beta-release/
tags:
  - Reflective Writing
  - Web Projects
---

Security cameras are looking good, adding HTML and CSS has gone smoothly so far. The website is now almost done, there is only the ghost data left to be displayed. This is quite difficult to show, as I have to rely on the camera not moving & causing the CSS to glitch out? I guess I can only show ghost information when the camera is paused, have it fade in slowly and fade out quickly on the camera being moved.

I fixed the mobile double tap not working bug with tocca.js, a handy library.

After getting more feedback from tutors and students, I have decided to add a drop down window that displays the information of selected character models and flowers. Having information directly overlayed onto the scene is very complicated to do well - I'd like to use CSS for a sharp graphical overlay, but that requires a live camera / css link, which I'd rather not get into. The drop down window can be toggled to show more / less on mobile.

I've added another canvas onto the window so I can render out a still from the scene of what the user has clicked on. I'd like to overlay some text on the canvas if possible? Just to save space. There should be a title, connection status (LIVE, GHOST), last connected, device identity. UI Design, here we go.