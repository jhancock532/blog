---
id: 235
title: 'Three.js &#8211; Movement, Collisions, Framing'
date: 2020-11-16T16:00:22+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=235
permalink: /three-js-movement-collisions-framing/
categories:
  - ThreeJS
  - Web Projects
---
We&#8217;re live! You can now test drive the website at <https://jhancock532.github.io/gallery/>. I&#8217;ve added keyboard controls to walk around, as well as basic collision detection so you can&#8217;t phase through walls.<figure class="wp-block-image size-large">

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/projector-effect-1024x576.jpg" alt="" class="wp-image-237" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/projector-effect-1024x576.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/projector-effect-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/projector-effect-768x432.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/projector-effect-1536x864.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/projector-effect.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />I&#8217;ve also added a new projector throw effect &#8211; a transparent material with Alpha Blending mode.<!--more-->

Playing with the gallery theme of plain white walls, open spaces, simple layouts, I mimic the context associated with an art space. This provides greater room for contemplation of gallery items, although providing video game style controls to navigate the space may detract from this. I&#8217;m using a shiny metallic gold material to frame important objects throughout the gallery.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="814" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Collision-Detection-Early-Testing-1024x814.jpg" alt="" class="wp-image-245" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Collision-Detection-Early-Testing-1024x814.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Collision-Detection-Early-Testing-300x238.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Collision-Detection-Early-Testing-768x610.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Collision-Detection-Early-Testing.jpg 1280w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />An early testing screenshot of collision detection. I&#8217;ve added stats.js (see top left) to see how well my code is performing.

Collision detection proved quite difficult at first, but it turns out I was over complicating things. I wanted to limit my character&#8217;s movement to within a certain polygon of space (which involves some tricky maths & manual calculation of the space boundaries) but then I discovered this <a href="http://stemkoski.github.io/Three.js/Collision-Detection.html" data-type="URL" data-id="http://stemkoski.github.io/Three.js/Collision-Detection.html">excellent tutorial on raycasting collision detection</a>. I added all the meshes in my scene as collision objects (apart from the projector light throw effect) and ta-da &#8211; it works! I have to thank SketchUp for automatically breaking up my model into seperate objects and ID&#8217;ing these objects for me with unique identifiers.

In the future I plan to add a collision slide effect, so when you collide with an object you don&#8217;t get stuck so easily. I&#8217;ve also discovered <a href="https://hofk.de/main/discourse.threejs/" data-type="URL" data-id="https://hofk.de/main/discourse.threejs/">an excellent tutorial series gathered from three.js discourse</a> which links to several interesting effects (object outline, raycasting from camera to interact with GLTF models with your mouse) that I&#8217;ll be implementing later.