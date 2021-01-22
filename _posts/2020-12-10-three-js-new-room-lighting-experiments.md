---
id: 273
title: 'Three.js &#8211; New Room, Lighting Experiments'
date: 2020-12-10T12:12:09+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=273
permalink: /three-js-new-room-lighting-experiments/
categories:
  - ThreeJS
  - Web Projects
---
I learned how to import models from the Sketch-Up asset store, and then how to explode them so that they successfully exported into Blender. In Blender I renamed and reorganised my object hierarchy, as this was getting messy.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="546" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/so-many-exploded-parts-to-organise-1024x546.jpg" alt="" class="wp-image-274" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/so-many-exploded-parts-to-organise-1024x546.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/so-many-exploded-parts-to-organise-300x160.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/so-many-exploded-parts-to-organise-768x409.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/so-many-exploded-parts-to-organise-1536x818.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/so-many-exploded-parts-to-organise.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> </figure> 

I then started experimenting with the different sources of lighting offered by Three.js. Ambient lighting helps give a base depth of light to my scene, I had issues with point lights being overly dramatic. The lighting doesn&#8217;t cast shadows correctly, perhaps a problem with my mesh travesal code, but I&#8217;m not overly worried about this. <figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="576" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/wild-spotlight-1024x576.jpg" alt="" class="wp-image-276" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/wild-spotlight-1024x576.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/wild-spotlight-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/wild-spotlight-768x432.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/wild-spotlight-1536x864.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/wild-spotlight.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> </figure> 

I decided to experiment with adding spotlights. I&#8217;ve noticed that point lights give the walls beautiful grading in colour, so I added a penumbra to my spotlight for a similar effect. <figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="576" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/spotlighteffect-1024x576.jpg" alt="" class="wp-image-279" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/spotlighteffect-1024x576.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/spotlighteffect-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/spotlighteffect-768x432.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/spotlighteffect-1536x864.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/spotlighteffect.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> </figure> 

Tweaking the roughness, lightness and metalic value of materials takes up a lot of time. It&#8217;s difficult to get the right feel, as this depends on how light is cast on the object, which is simulated differently in Three.js and in Blender.

I intend to add a further room to the gallery, then a corridor &#8211; as my development time is now entering the final stages of the project with two months to go, I&#8217;d like to give myself plenty of time to do front-end UI pages and a mobile friendly website.