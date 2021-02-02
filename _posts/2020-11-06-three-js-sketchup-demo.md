---
id: 210
title: 'Web Tech - SketchUp Is Still Free'
date: 2020-11-06T17:46:18+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=210
permalink: /three-js-sketchup-demo/
tags:
  - ThreeJS
  - Web Projects
---
<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Low-Triangle-Success-1024x541.jpg" alt="" class="wp-image-211" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Low-Triangle-Success-1024x541.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Low-Triangle-Success-300x159.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Low-Triangle-Success-768x406.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Low-Triangle-Success-1536x812.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Low-Triangle-Success.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />
Low Poly Museum Creation

For low poly designs, SketchUp is excellent for quick model creation. There is a free edition available to download still ([SketchUp Make 2017](https://www.sketchup.com/download/all)), this allows for OBJ file exports. Unfortunately, none of the textures I tried to export with this file made it through &#8211; I tried adding textures in Blender, but no luck there either. This hopefully won&#8217;t be a difficult issue to resolve.

<!--more-->

I&#8217;m now developing locally using a VSCode extension to host and serve my files. This gets around a lot of CORS request pain & using GitHub to host models.

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/No-Shading-Luck-However-1024x576.jpg" alt="" class="wp-image-212" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/No-Shading-Luck-However-1024x576.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/No-Shading-Luck-However-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/No-Shading-Luck-However-768x432.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/No-Shading-Luck-However-1536x864.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/No-Shading-Luck-However.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />The model successfully loads in Three.js

The shading for some of the walls works, but not all of them. This is an interesting error &#8211; perhaps not all walls are double sided, and this is something to be careful of?

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-1024x346.jpg" alt="" class="wp-image-213" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-1024x346.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-300x101.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-768x259.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-1536x518.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Successful-Implementation-of-First-Person-Controls-Rather-Sickening-2048x691.jpg 2048w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />Successful implementation of FirstPersonControls.js

FirstPersonControls.js is a horrible camera controller. I can see why they haven&#8217;t given an example for it in the documentation, I feel sick using it. I spent a lot of time failing to import an older version of the library, luckily GitHub delivered the goods. What I actually want are [PointerlockControls](https://threejs.org/docs/#examples/en/controls/PointerLockControls), &#8220;the perfect choice for first person 3D games&#8221;.

Next time I&#8217;ll implement the PointerLockControls and play more with materials &#8211; I&#8217;d love to paint these on and customise them in Blender, ideally with bump maps for nicer texture effects.