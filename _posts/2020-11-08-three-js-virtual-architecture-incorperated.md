---
id: 218
title: 'Three.js &#8211; Virtual Architecture Incorperated'
date: 2020-11-08T15:25:58+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=218
permalink: /three-js-virtual-architecture-incorperated/
categories:
  - ThreeJS
  - Web Projects
---
Web development has never felt so strange &#8211; the entire focus of the project is utilising and styling 3D space. Plenty of design choices to be made! Here&#8217;s my working so far&#8230;

<!--more-->

Due to the constrictive nature of lockdown, I&#8217;ve chosen to make my gallery as open and airy as possible &#8211; this makes a nice change from the cramped living conditions that are typical for student accomodation. Due to the content heavy nature of the internet, I&#8217;ve chosen to showcase only one piece of artwork per room, hoping to avoid content overload syndrome. The main room of the gallery has the projector box placed at the center of the space; I like having its presence highlighted, I like the idea of revealing the system that supports the scene. This is why I&#8217;ve added a window to the back of the gallery room &#8211; a window looking out into nothingness, the black void of the rendering engine!<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="517" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Welcome-to-the-glTF-specification-1024x517.jpg" alt="" class="wp-image-220" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Welcome-to-the-glTF-specification-1024x517.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Welcome-to-the-glTF-specification-300x151.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Welcome-to-the-glTF-specification-768x388.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Welcome-to-the-glTF-specification-1536x775.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Welcome-to-the-glTF-specification.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />I&#8217;m loading my model via the .glTF file format &#8211; the above is the file format specification, I scanned over this to learn about my limitations / creative license whilst modelling.

From the above I wasted an hour trying to load in a normal map to make the wall textures look more painted. I&#8217;ll return to this later.<figure class="wp-block-image size-large is-resized">

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Not-Much-Luck-with-The-Normal-Map-1024x578.jpg" alt="" class="wp-image-221" width="674" height="380" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Not-Much-Luck-with-The-Normal-Map-1024x578.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Not-Much-Luck-with-The-Normal-Map-300x169.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Not-Much-Luck-with-The-Normal-Map-768x434.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Not-Much-Luck-with-The-Normal-Map.jpg 1510w" sizes="(max-width: 674px) 100vw, 674px" />This isn&#8217;t what the normal map is supposed to look like.

Much more successful was adding the emission texture via tweaking a material.<figure class="wp-block-image size-large is-resized">

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Added-Emission-To-The-Projector-Wall-1024x696.jpg" alt="" class="wp-image-219" width="674" height="458" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Added-Emission-To-The-Projector-Wall-1024x696.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Added-Emission-To-The-Projector-Wall-300x204.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Added-Emission-To-The-Projector-Wall-768x522.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Added-Emission-To-The-Projector-Wall.jpg 1189w" sizes="(max-width: 674px) 100vw, 674px" />I added emission to the projector throw space so it renders brightly.

Finally, I loaded the scene and added basic PointerLockControls for the camera movement system. Next week I&#8217;ll be making the site live on GitHub Pages so you can play with it yourself &#8211; until then, plenty of thought needs to go into gallery layout&#8230;<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="786" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Online-Emissive-1024x786.png" alt="" class="wp-image-222" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Online-Emissive-1024x786.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Online-Emissive-300x230.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Online-Emissive-768x590.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/11/Online-Emissive.png 1276w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />And the lighting system, and making textures less shiny, and&#8230;</figure>