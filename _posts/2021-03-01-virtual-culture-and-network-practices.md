---
title: Virtual Culture and Network Practices
project: Network Practices
date: 2021-02-02T14:42:39+00:00
author: James
layout: post
permalink: /virtual-culture-and-network-practices/
tags:
  - Reflective Writing
  - Web Projects
---

The learning outcomes for this unit:

 - **LO1** - show insight into network technologies and digital media arts practices relating to your own areas of personal interest, expertise and research;
 - **LO2** - describe the development and production of an experimental network project that shows a substantial and coherent level of research;
 - **LO3** - demonstrate that you have understanding of professional and cultural practices, and the development of virtual networks;


*Whether through web based, mobile or integrated technology forms, students will research and develop a simple project using network structures to create innovative approaches to media generation, interaction and dissemination that support new cultural social and communications in the digital age.*

### Assessment
Each student will present a summative critical presentation (20 minutes), a visual demonstration of the working on line project and a reflective commentary situating the work in the wider critical context of social media and and the development of virtual networks

## My Intended Learning Plan

Develop a website which shows the presence of other people visiting the website. 

- Display a group of virtual 3D humans for each member online, reminding us of the physical people we are networked with.
- Show a selection of ghosts of people who have visited the website in the past, demonstrating the temporal disconnect of our online networks, perhaps also the loneliness and disconnect of the internet.
- Modify each individual's 3D avatar via a hash of their browser fingerprint, revealing the often hidden but distinguishing digital presence we have whilst networked online.

Further considerations:
- Allow the API of the website to be publicly accessible and the source code easily duplicated so that "presence" on the website is truely distributed online. In the spirit of No Fun, the website could get DDOS'd and taken down as it gains public attention; this is in the nature of the network.

Social Media Hype:
- Create a few progress posts for social media, ideally showcasing fancy graphics.
- Share progress in the Essay Games discord server - having shared labyr.in/th/ there some people have already enjoyed my work.
- Continue my exploration of Twitter and my deep dive into existing web communities. I have found several contemporaries and I have been contributing to their work ([Tim Holmans' puginarug.com](https://github.com/tholman/puginarug/pull/1), [Estela A.Ortiz's Collaborative Book](https://github.com/e-aortiz/collaborative-book/pull/1)), in the meantime I have been following and messaging Twitter accounts with similar interests to me. These small interactions gradually build up over time.
- I will invite various people to participate in my website a week before the event, and publise it widely. I hope that the tweet invitation itself only receives a dozen or so interactions, as I don't intend for 1000's of people to join all at once. The server could probably handle it, but the website would get cluttered.

# Technical Requirements

## Server

I have a little experience of server side web development from my time at Bristol, however real-time connections between server and client is something new to me.

In my preliminary research I have decided to use Backendless to host my website database and API. After completing several hours of tutorials, Backendless offers registrants a free server hosting plan with unlimited API calls and generous database storage.

They also offer access to a Real Time API; this API stores data to a quickly accessible database and pushes notifications of updated data to clients. Clients can push, update and delete data from the server as necessary - I intend to use this to monitor currently active presences.

I have explored the Codeless REST API scripting tools provided by Backendless; I've used them to set up a simple "new participant register" POST API request, as well as a GET request to see previous site visitors. I intend to adjust this GET request with some logic to select and return a variety of previous participants from a diverse time span.

## Fingerprints

Having researched fingerprinting, I find that there are many solutions online, but only one major open-source option: fingerprint.js. This site offers 60% idenitification accuracy for its free tier, so I am tempted to copy the fingerprinting code from other research sites to get a higher accuracy.

[A good website to steal fingerprinting code from perhaps?](https://amiunique.org/fp) - After looking at the code, there was too much noise. I have decided to use a less effective method, it will probably be good enough to distinguish users.

[Another open source fingerprinting repository, browser fingerprint](https://github.com/actionhero/browser_fingerprint) - Sadly, this tool doesn't provide canvas fingerprinting. This is a shame because font data contains a lot of unique information.

Although I am sad to use a library that is not truely open source, I will use fingerprint.js for this project.

## WebPack / SnowPack

I would like to keep dependancies low for this project, but after the first 3D project I recognise the importance for NPM to look after my libraries for me. I will use SnowPack to prioritise speed over total number of HTTPS requests. It is unlikely that I will need to use Glup to concat or minify any of my JS, so I shall avoid this for now.

I intend to provide the participant with no user interface, so I am not going to use Sass for this project - there is very little styling necessary.

I have never used SnowPack before, nor have I used WebPack. I am relatively new to Node.js so I expect that this will slow down my project development.




<!--![Image of a big 12 in the gallery room](/blog/wp-content/uploads/meta-data/big-12.jpg)-->
