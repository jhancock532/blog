---
id: 254
title: 'Three.js &#8211; Menu Overlay, Object Highlighting'
date: 2020-11-24T15:28:02+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=254
permalink: /three-js-menu-overlay-object-highlighting/
tags:
  - ThreeJS
  - Web Projects
---
<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/homemenuoverlay-1024x569.jpg" alt="" class="wp-image-255" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/homemenuoverlay-1024x569.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/homemenuoverlay-300x167.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/homemenuoverlay-768x427.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/homemenuoverlay-1536x854.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/homemenuoverlay.jpg 1928w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /><figcaption>A simple home menu overlay.

I&#8217;m reconsidering the placement of the &#8220;Visit the Gallery&#8221; button, as it obscures the bottom of the scrolling section on the left. Otherwise I&#8217;m happy with the font choice, EBGaramond. This is my first time using a variable font for a project, I&#8217;d like to experiment more with variable font properties&#8230;

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/take-a-closer-look-1024x701.jpg" alt="" class="wp-image-256" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/take-a-closer-look-1024x701.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/take-a-closer-look-300x205.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/take-a-closer-look-768x526.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/take-a-closer-look.jpg 1279w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />A quick draft of looking closely at things.

I&#8217;m using Three.JS BoxHelper to outline this object, along with a simple magnifying glass <img> overlayed on the screen. The red outline isn&#8217;t that visible, so I might start investigating [post-processing render tasks](https://threejs.org/examples/?q=outline#webgl_postprocessing_outline) (which involves a fair few more JavaScript files) to get a better outline glow effect. Ideally I don&#8217;t want to have to use a magnifying glass in the final result.