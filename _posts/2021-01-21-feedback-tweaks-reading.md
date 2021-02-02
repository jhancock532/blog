---
id: 306
title: Labyr.in/th/ - Feedback, Tweaks, Reading
date: 2021-01-21T14:42:39+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=306
permalink: /feedback-tweaks-reading/
tags:
  - Reading
  - Reflective Writing
  - Web Projects
---
There&#8217;s ten days before my final submission deadlines for web technology and interactive installations. I&#8217;ve got feedback on labyrinth and a list of things to do for the personal website, which I&#8217;m steadily working through day by day.

On chatting to people about the form of personal websites, I recognise the desire of site visitors to quickly see what I&#8217;ve created, as opposed to having to navigate a complex interface. Accordingly, I&#8217;m adding a basic showreel page to the site, this containing a simple array of pictures. The showreel will be the first link on my homepage to add to its prominence, followed by a link to labyrinth.

The lighting effects in the gallery cause immense lag when multiplied; after investigating how to bake the lighting in Blender for an hour, I gave up &#8211; I also considered adding textures to the walls, but I considered the cost of learning texture mapping, then going through the model, a bit outside the scope of the time I have left.

I will do some of the things recommended at <https://discoverthreejs.com/tips-and-tricks/> for the final polishing of the gallery; I have currently added three exhibits, this will likely be all that I am showcasing. Writing up the exhibit description pages is also an important step in the process.

After getting feedback on labyrinth from a variety of sources, including coursemates, tutors and game design tutors from other universities, I&#8217;ve decided to add sound effects to the scroll webpages. Ideally I&#8217;d also add mobile device detection and auto skip buttons for impossible mobile sections, but that will have to wait.

My reading is based on Net Art and source code commentary. I was interested to find that some of jodi&#8217;s webart is based on source code comments, and how they aren&#8217;t particularly fussed as a duo as to whether there work is considered art or not. I am intrigued by the role of the human interacting with the website, as I find the deadness of the screen not as interesting as the vibrancy of the lived experience.

In the asethic of failure; net art gone wrong, there was an interesting comment on Luining&#8217;s work &#8211;

<blockquote class="wp-block-quote">
  <p>
    <em>Luining dismantles the spectator&#8217;s ability to determine things by actually allowing a high level of engagement or &#8216;interactivity&#8217;.</em>
  </p>
</blockquote>

This suggests that if you&#8217;re distracted or playing a part, your ability to discern is clouded. This follows the nature of the web 2.0 &#8211; acting in a goal oriented manner, or to be idly entertained. Perhaps the lens and immediate interactive intimacy of the screen, mouse, keyboard lends itself for us to interact with all web experiences as either of the two manners, therefore no net art? Found a good book on the body in relation to the internet, will be reading that soon &#8211; after another go at The Work Of Art In The Age Of Mechanical Reproduction.

Luther Blissett maintains that net art is &#8220;Everyone with his own site, everyone with his own domain, everyone with his own gallery, they are throwing themselves into the trammels of traditional art.&#8221;

This is a lovely quote, I shall make sure to make my website gallery slightly tongue in cheek with a YouTube play button in the corner somewhere, and a live figure of the number of subscribers I have.

After having a tutor try and go through the site on a Mac and trackpad, I realised the importance of device specific interaction indicators. On Mac devices the close window button is on the left hand side, and the back button isn't in the same place in the browser UI. There's a further problem in that the scroll bar isn't visible when you're scrolling sideways, which means `going.html` doesn't function at all. I've redrawn interaction indicators and skipped the `going.html` page entirely for mac devices. I will however restrict visitors of the site (who are marking) to follow a list of instructions very carefully before starting and during the experience. Using a trackpad can result in visitors unintentionally going back or forward a webpage, breaking the order of the site - hence, the trackpad is banned, and a mouse is to be used instead.

Because I find the idea of someone visiting the site on their Amazon Fire TV stick interesting / I want my labyrinth to be performed across as many devices as possible, I've added in automatic time out skips if the visitor isn't able to complete the webpage task. Having this inevitablity of direction is very important to the idea of a labyrinth also.

Considering the accessibility of the site, I am very aware that there is none. No tags, descriptions, explainers, keyboard focus elements, etc. I wish I had more time to add a little story into each webpage for TTS visitors.

I've ported over my blog from WordPress to jekyll with GitHub Pages. This is much better, I prefer static with HTTPS over security risks with lag any day.

