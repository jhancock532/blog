---
id: 200
title: 'Three.js &#8211; Just Getting Started'
date: 2020-11-04T19:20:04+00:00
author: James
layout: post
guid: http://www.jameshancock.art/?p=200
permalink: /diving-into-three-js/
categories:
  - ThreeJS
  - Web Projects
---
For the Web Technologies unit on this course I intend to make a 3D portfolio site, a gallery you can walk around to view my artwork. I&#8217;m rather new to Three.js, so I&#8217;ll be working from the tutorial guides to start off. Here are some things I&#8217;ve learned&#8230;

<!--more-->

Don&#8217;t load a 23MB file for your first GLB file loading demo. It will take ages and won&#8217;t look good, especially if you&#8217;re spending your object file from GitHub raw to CodePen.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="823" src="http://www.jameshancock.art/wp-content/uploads/2020/11/That-Loading-Though-1024x823.png" alt="" class="wp-image-201" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/That-Loading-Though-1024x823.png 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/That-Loading-Though-300x241.png 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/That-Loading-Though-768x617.png 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/That-Loading-Though.png 1200w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>The black area covering the default cube is my model. It took roughly a minute to load.</figcaption></figure> 

Don&#8217;t test with a 100% metalic object if you haven&#8217;t got a directional light in your scene. Do test with a really easy and quick to load 45kB file.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="781" src="http://www.jameshancock.art/wp-content/uploads/2020/11/Just-Like-That-1024x781.jpg" alt="" class="wp-image-202" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/Just-Like-That-1024x781.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/Just-Like-That-300x229.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/Just-Like-That-768x585.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/Just-Like-That.jpg 1275w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> </figure> 

Don&#8217;t immediately jump into the first person camera controls &#8211; these are difficult. Try doing lighting first, so you can see where you&#8217;re going.

And viola &#8211; my first Three.js scene. Click and drag in the window to look around, scrolling zooms in and out.

<p class="codepen" data-height="550" data-theme-id="dark" data-default-tab="result" data-user="jhancock532" data-slug-hash="jOrpNOM" style="height: 550px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Three.js Model Loading, Shading, Animation Demo">
  <span>See the Pen <a href="https://codepen.io/jhancock532/pen/jOrpNOM"> Three.js Model Loading, Shading, Animation Demo</a> by James Hancock (<a href="https://codepen.io/jhancock532">@jhancock532</a>) on <a href="https://codepen.io">CodePen</a>.</span>
</p>