---
title: 'Bringing A Mysterious House Online'
project: Web Tech
date: 2020-12-08T18:03:14+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=265
permalink: /three-js-bringing-a-mysterious-house-online/
tags:
  - ThreeJS
  - Web Projects
---
I&#8217;m a long time fan of [DearestHershel](https://www.youtube.com/channel/UCJneOHw09N_K1eXmtEWSgBA), a Professor Layton fan meme channel. Watching the 2K subs special, I saw that Bob had used a 3D model of the room whilst creating the video. I wondered if I could convert that room into an online space &#8211; then I hit Bob up on Discord to ask for the assets. Here&#8217;s what I learned from two day project.

Creating scenes for the web is a pain. You have to reduce all the assets texture sizes and polygon counts, I did this using Blender.

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/bobs-model-early-import-1024x527.jpg" alt="" class="wp-image-266" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/bobs-model-early-import-1024x527.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/bobs-model-early-import-300x154.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/bobs-model-early-import-768x395.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/bobs-model-early-import-1536x790.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/bobs-model-early-import.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />Importing the OBJ&#8217;s taught me how to apply textures.

  * Why would we use a 8MB texture for bookshelves?
  * We can duplicate instances of the sofa so we don&#8217;t need double the mesh data
  * I&#8217;ve reduced the size of the sofa texture in half, saved it as a jpeg, made it lighter
  * I&#8217;m limiting image file sizes to 100kb, 1024 by 1024 and shifting the jpeg compression quality to 60%.

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/prototyping-in-the-threejs-editor-1024x576.jpg" alt="" class="wp-image-267" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/prototyping-in-the-threejs-editor-1024x576.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/prototyping-in-the-threejs-editor-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/prototyping-in-the-threejs-editor-768x432.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/prototyping-in-the-threejs-editor-1536x864.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/prototyping-in-the-threejs-editor.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />I prototyped early exports of material textures using the online three.js editor, as well as lighting effects.

  * The curtains are super big &#8211; used the decimate function, mode planar, to reduce the triangle count down to 1700 (from 6500) without large drop in quality.
  * Ok &#8211; exported object file looking super big at 16MB 🙁
  * With default compression settings, 15MB
  * Maybe everything could be scaled down? Less large floats to worry about?
  * Chosing to export images as jpeg cut the file size down to 4.5MB! That&#8217;s like the size of a normal bloated webpage!

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/off-scaling-1024x576.jpg" alt="" class="wp-image-268" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/off-scaling-1024x576.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/off-scaling-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/off-scaling-768x432.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/off-scaling-1536x864.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/off-scaling.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />I imported the scene horribly overscaled into my original gallery website, then I started gutting out code.

  * It is incredibly disorientating to see another mouse move across your webpage. Like seriously weird, even if it&#8217;s in a background video that&#8217;s projected onto a 3D scene.
  * Adding lots of small details really fills out a scene.
  * I can make textures reflective! Not sure that it will export to GLB though&#8230; it kinda did? lights reflect, but not the environment. It kinda looks like a mirror, maybe.
  * Textures still look ok at 512 by 512, depends on size of file I guess.
  * I reused the door texture for the table. It looks fine.

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/Brilliant-1024x576.jpg" alt="" class="wp-image-269" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/Brilliant-1024x576.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/Brilliant-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/Brilliant-768x432.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/Brilliant-1536x864.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/Brilliant.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />After messing with increasing light intensity, I then scaled the entire model down.

  * This is good practice for playing with different material effects. GLB files have to use roughness and metallic effects, I can&#8217;t use specular.
  * For minor details, don&#8217;t import image textures, just use materials.
  * Metalic textures are awesome!
  * Small props added, file size now 17MB &#8211; scalling the file down actually increased the size of the file by 5 kb. I&#8217;ve applied compression, not sure how this will effect how the model displays.

<img loading="lazy" width="967" height="124" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/ive-broken-the-universe.jpg" alt="" class="wp-image-270" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/ive-broken-the-universe.jpg 967w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/ive-broken-the-universe-300x38.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/ive-broken-the-universe-768x98.jpg 768w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />Plenty of bugs. This is a slap dash project, so this is slap dash documentation. Time doesn&#8217;t exist to a compiler.

  * <a rel="noreferrer noopener" target="_blank" href="https://threejs.org/docs/#examples/en/loaders/DRACOLoader">https://threejs.org/docs/#examples/en/loaders/DRACOLoader</a> &#8211; Draco compression looks cool, giving it a go.
  * And&#8230; I only saved a couple hundred kb in comparision to the compression offered by Blender. Ah well.

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/project-bob-finale-1024x576.png" alt="" class="wp-image-271" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/12/project-bob-finale-1024x576.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/project-bob-finale-300x169.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/project-bob-finale-768x432.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/project-bob-finale-1536x864.png 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/12/project-bob-finale.png 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />The final result! This site only works on Firefox, for some reason glitches occur on other people&#8217;s PC&#8217;s. Ah well, mission accomplished.

Check it out at <https://jhancock532.github.io/cosy-room/>