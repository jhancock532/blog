---
id: 298
title: 'Labyr.in/th/ &#8211; Finishing Touches'
date: 2021-01-08T12:30:41+00:00
author: James
layout: post
guid: http://www.jameshancock.art/?p=298
permalink: /labyr-in-th-finishing-touches/
categories:
  - Reflective Writing
  - Web Projects
---
Inspired by URL creativity, for example waveyurl.com, I&#8217;ve added a secret mirrored URL within my website. Testing my site across multiple browsers, I noticed that Chome renders any whitespace character in the URL bar as %20 &#8211; this meant that I had to change the URL basis for my site to another character, switching from `labyr.in/th/ entrance.html` to `labyr.in/th/ㅡentrance.html`. Testing on Chrome I noticed that my site performed markedly better, especially regarding audio performance.

<!--more--><figure class="wp-block-image size-large">

<img loading="lazy" width="879" height="844" src="http://www.jameshancock.art/wp-content/uploads/2021/01/the-labyrinth-dance.png" alt="" class="wp-image-299" srcset="http://www.jameshancock.art/wp-content/uploads/2021/01/the-labyrinth-dance.png 879w, http://www.jameshancock.art/wp-content/uploads/2021/01/the-labyrinth-dance-300x288.png 300w, http://www.jameshancock.art/wp-content/uploads/2021/01/the-labyrinth-dance-768x737.png 768w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> </figure> 

Searching the internet archive, I found a piece of sheet music from the 1800&#8217;s named &#8220;The Labyrinth&#8221;. This music is the soundtrack of the center of the labyrinth, its light and playful nature reflecting the joyful use of labyrinths in celebration and games at that time. Sound is vital throughout the site. Without sound, pages such as `ㅡsliding.html` are rather boring.

Taking inspiration from <a href="http://best.effort.network" data-type="URL" data-id="best.effort.network">best.effort.network</a>, I updated the favicon of my site dynamically from white to black to indicate the state change of the website. 

I&#8217;ve noticed that if you click refresh a few times at the wrong points in the website, the logic and flow of the site will break. If the logic breaks completely, the visitor will be redirected to `/undefined/`, the error value returned by a JavaScript function. Instead of fixing the logic of the site, I&#8217;ve added an index.html file that you reach when you navigate to `/undefined/`. This site is meant to be performed and explored interactively, and that means breaking it, modifying it, looking at source code, just as much as following the intended path.

I&#8217;ve hidden a person at `/img/index.html` as an easter egg. &#8220;The developer coded humanity in their own image.&#8221;

I&#8217;m curating how the site is performed in Google Search results through adding noindex and nofollow meta tag to any webpage that isn&#8217;t a valid entry point to my site. I&#8217;m also adding a robots.txt file to further unindex webpages.

Monitoring the performance of the website across social media is another thing I looked into &#8211; <https://metatags.io/> helped me realise that I could make my site display in different ways when it was linked on Twitter and Facebook.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="514" src="http://www.jameshancock.art/wp-content/uploads/2021/01/image-1024x514.png" alt="" class="wp-image-300" srcset="http://www.jameshancock.art/wp-content/uploads/2021/01/image-1024x514.png 1024w, http://www.jameshancock.art/wp-content/uploads/2021/01/image-300x151.png 300w, http://www.jameshancock.art/wp-content/uploads/2021/01/image-768x385.png 768w, http://www.jameshancock.art/wp-content/uploads/2021/01/image.png 1497w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> </figure> 

This gives me an idea for a site that is performed dynamically each time someone links to it on social media. Posts from a story perhaps, or simply a quote of the day app? I wonder how Twitter and Facebook&#8217;s caching system would interfere.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="537" src="http://www.jameshancock.art/wp-content/uploads/2021/01/image-1-1024x537.png" alt="" class="wp-image-301" srcset="http://www.jameshancock.art/wp-content/uploads/2021/01/image-1-1024x537.png 1024w, http://www.jameshancock.art/wp-content/uploads/2021/01/image-1-300x157.png 300w, http://www.jameshancock.art/wp-content/uploads/2021/01/image-1-768x402.png 768w, http://www.jameshancock.art/wp-content/uploads/2021/01/image-1.png 1456w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> </figure> 

I&#8217;ve had the above idea in my head for a while now, so I thought I might throw it in as an easter egg if someone tries to link to `labyr.in/th/ㅡindex.html` on social media. Reference to Island by Aldous Huxley.

In the messiness of code, there is humanity. A creator hiding behind the if statements. As such, I am curating the commentary and ugliness of my code to a minimum. I also need to save time.

Time to publish and get feedback.