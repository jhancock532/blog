---
id: 238
title: 'Three.js &#8211; Movement, Framing'
date: 2020-11-12T16:13:25+00:00
author: James
layout: revision
guid: http://www.jameshancock.art/235-revision-v1/
permalink: /235-revision-v1/
---
 

You can now test drive the website at <https://jhancock532.github.io/gallery/>. I&#8217;ve added keyboard controls (with sprinting) to walk around, currently there isn&#8217;t any collision detection so don&#8217;t be afraid if you start phasing through walls.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="576" src="http://www.jameshancock.art/wp-content/uploads/2020/11/projector-effect-1024x576.jpg" alt="" class="wp-image-237" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/projector-effect-1024x576.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/projector-effect-300x169.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/projector-effect-768x432.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/projector-effect-1536x864.jpg 1536w, http://www.jameshancock.art/wp-content/uploads/2020/11/projector-effect.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>I&#8217;ve also added a new projector throw effect &#8211; a transparent material with Alpha Blending mode.</figcaption></figure> 

As I&#8217;m creating a gallery, I&#8217;m also curating its contents. Playing with the gallery theme (plain white walls, open space, simplistic layout) I have access to the gallery context, the mental space you enter when visiting an art space. In this art space, there is greater room for contemplation (especially if the contents of the gallery are spaced out and limited in number). To indicate what I find worthy of contemplation, I&#8217;m using a shiny metallic gold frame material.

I love the idea of looking into the void of the rendering engine, the default value to be drawn as no rays have intersected in this section of the canvas.