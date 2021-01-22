---
id: 231
title: 'Three.js &#8211; SketchUp Is Still Free'
date: 2020-11-09T16:41:11+00:00
author: James
layout: revision
guid: http://www.jameshancock.art/210-revision-v1/
permalink: /210-revision-v1/
---
 <figure class="wp-block-image size-large"><img loading="lazy" width="1024" height="541" src="http://www.jameshancock.art/wp-content/uploads/2020/11/Low-Triangle-Success-1024x541.jpg" alt="" class="wp-image-211" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/Low-Triangle-Success-1024x541.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/Low-Triangle-Success-300x159.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/Low-Triangle-Success-768x406.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/Low-Triangle-Success-1536x812.jpg 1536w, http://www.jameshancock.art/wp-content/uploads/2020/11/Low-Triangle-Success.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /><figcaption>Low Poly Museum Creation</figcaption></figure> 

For low poly designs, SketchUp is excellent for quick model creation. There is a free edition available to download still ([SketchUp Make 2017](https://www.sketchup.com/download/all)), this allows for OBJ file exports. Unfortunately, none of the textures I tried to export with this file made it through &#8211; I tried adding textures in Blender, but no luck there either. This hopefully won&#8217;t be a difficult issue to resolve.

<!--more-->

I&#8217;m now developing locally using a VSCode extension to host and serve my files. This gets around a lot of CORS request pain & using GitHub to host models.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="576" src="http://www.jameshancock.art/wp-content/uploads/2020/11/No-Shading-Luck-However-1024x576.jpg" alt="" class="wp-image-212" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/No-Shading-Luck-However-1024x576.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/No-Shading-Luck-However-300x169.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/No-Shading-Luck-However-768x432.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/No-Shading-Luck-However-1536x864.jpg 1536w, http://www.jameshancock.art/wp-content/uploads/2020/11/No-Shading-Luck-However.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>The model successfully loads in Three.js</figcaption></figure> 

The shading for some of the walls works, but not all of them. This is an interesting error &#8211; perhaps not all walls are double sided, and this is something to be careful of?<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="346" src="http://www.jameshancock.art/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-1024x346.jpg" alt="" class="wp-image-213" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-1024x346.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-300x101.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-768x259.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-1536x518.jpg 1536w, http://www.jameshancock.art/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-2048x691.jpg 2048w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>Successful implementation of FirstPersonControls.js</figcaption></figure> 

FirstPersonControls.js is a horrible camera controller. I can see why they haven&#8217;t given an example for it in the documentation, I feel sick using it. I spent a lot of time failing to import an older version of the library, luckily GitHub delivered the goods. What I actually want are [PointerlockControls](https://threejs.org/docs/#examples/en/controls/PointerLockControls), &#8220;the perfect choice for first person 3D games&#8221;.

Next time I&#8217;ll implement the PointerLockControls and play more with materials &#8211; I&#8217;d love to paint these on and customise them in Blender, ideally with bump maps for nicer texture effects.