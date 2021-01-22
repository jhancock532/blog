---
id: 230
title: 'Three.js &#8211; Project Projector'
date: 2020-11-09T16:39:57+00:00
author: James
layout: revision
guid: http://www.jameshancock.art/225-revision-v1/
permalink: /225-revision-v1/
---
 

I was having difficulty loading in the video texture until I figured out that the Geometry plane was facing away from me &#8211; thankfully, a quick rotation sorted this out. Along the way I copied a few [Three.js examples](https://threejs.org/examples/?q=video#webgl_video_panorama_equirectangular), creating the horrifying sphere of social media content. Framing the content in this form it is completely overwhelming.

<!--more--><figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="819" src="http://www.jameshancock.art/wp-content/uploads/2020/11/DebuggingTheProjectorMesh-1024x819.png" alt="" class="wp-image-226" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/DebuggingTheProjectorMesh-1024x819.png 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/DebuggingTheProjectorMesh-300x240.png 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/DebuggingTheProjectorMesh-768x614.png 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/DebuggingTheProjectorMesh.png 1281w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>Ahhhhhhhhhhh, not the sphere!</figcaption></figure> 

After hurdling &#8220;it&#8217;s facing the wrong way&#8221; things went very smoothly. I&#8217;ve built my 3D model very precisely in SketchUp (to the nearest meter or 10cm) and as Three.js works with meters as its default scaling, I haven&#8217;t had to do any awkward maths.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="820" src="http://www.jameshancock.art/wp-content/uploads/2020/11/The-Wall-Of-Tweets-Is-Alive-1024x820.jpg" alt="" class="wp-image-227" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/The-Wall-Of-Tweets-Is-Alive-1024x820.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/The-Wall-Of-Tweets-Is-Alive-300x240.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/The-Wall-Of-Tweets-Is-Alive-768x615.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/The-Wall-Of-Tweets-Is-Alive.jpg 1276w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>The wall of tweets, V1</figcaption></figure> 

After loading and positioning the projector mesh, I added a basic emission to it&#8217;s material to make it look a little brighter. The background wall emission doesn&#8217;t pass through, so I can delete this face in future editions of the 3D model file. A cool thing to note though is that I can add an alpha transparency map &#8211; perhaps a nice projector pixelation effect would add to the atmosphere here?<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="604" src="http://www.jameshancock.art/wp-content/uploads/2020/11/Material-Emissions-Applied-to-Projector-1024x604.jpg" alt="" class="wp-image-228" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/Material-Emissions-Applied-to-Projector-1024x604.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/Material-Emissions-Applied-to-Projector-300x177.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/Material-Emissions-Applied-to-Projector-768x453.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/Material-Emissions-Applied-to-Projector-1536x907.jpg 1536w, http://www.jameshancock.art/wp-content/uploads/2020/11/Material-Emissions-Applied-to-Projector.jpg 1816w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>Swapped to a Lambert material, added basic emission.</figcaption></figure> 

The final touch will be to add a transparent mesh mimicing the throw of the projector through dust. This could flicker slightly, along with a light in the projector source box. Hopefully these two steps will be enough to convert the black cube in the center of the stage from a box to a projector &#8211; else I&#8217;ll have to do some more 3D modelling!<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="808" src="http://www.jameshancock.art/wp-content/uploads/2020/11/Cannot-tell-if-black-texture-or-just-the-void-1024x808.jpg" alt="" class="wp-image-229" srcset="http://www.jameshancock.art/wp-content/uploads/2020/11/Cannot-tell-if-black-texture-or-just-the-void-1024x808.jpg 1024w, http://www.jameshancock.art/wp-content/uploads/2020/11/Cannot-tell-if-black-texture-or-just-the-void-300x237.jpg 300w, http://www.jameshancock.art/wp-content/uploads/2020/11/Cannot-tell-if-black-texture-or-just-the-void-768x606.jpg 768w, http://www.jameshancock.art/wp-content/uploads/2020/11/Cannot-tell-if-black-texture-or-just-the-void.jpg 1272w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>The window at the front of the gallery. Is it a black texture, or is it the void?</figcaption></figure>