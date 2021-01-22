---
id: 143
title: Webcam Presence
date: 2020-10-16T09:36:17+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=143
permalink: /webcam-presence/
categories:
  - Web Projects
---
You&#8217;re being watched &#8211; by yourself.

Social media is often used as a form of escapism, with plenty of passive entertainment to distract us from the everyday. While I&#8217;m scrolling through Twitter or Reddit, I don&#8217;t pay much attention to anything much other than the content that&#8217;s in front of me, making it easy to get lost in the unending train tracks of internet information, clicking on links to the latest trends, catching up with my favourite profiles.

This is the opposite to mindfulness practice; lost in the flow, we&#8217;re temporarily disconnected from reality. How might we experiment with bringing presence to our scrolling? 

<!--more-->

I&#8217;d like to experiment with using a webcam, to place myself directly in or beside the content in clear view so that I have a reminder of reality, no matter how far down I scroll. Getting access to the webcam and duplicating the steam to multiple video sources is relatively easy. <a href="https://codepen.io/jhancock532/pen/wvWMYrv" data-type="URL" data-id="https://codepen.io/jhancock532/pen/wvWMYrv">Click here to see the live demo with source code</a>.

To take these video elements and insert them into Twitter requires a FireFox extension. This is where things get complicated; for some reason, Twitter automatically applies some JavaScript to all new video objects added to the webpage, resetting their stream. Whenever a stream object is added, the JavaScript removes it again. My solution to this problem was to continually add the webcam stream to the video element &#8211; causing a flickering video to appear. To resolve the flicker issue, I decided to paint the video stream to a canvas element; as a result of which, I realised I could control the opacity of the canvas to make my face overlay the screen entirely.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="572" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/fadingpresence-1024x572.jpg" alt="" class="wp-image-146" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/fadingpresence-1024x572.jpg 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/fadingpresence-300x168.jpg 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/fadingpresence-768x429.jpg 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/fadingpresence-1536x858.jpg 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/fadingpresence.jpg 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>The Magic Mirror</figcaption></figure> 

I chose to have the webcam opacity fade in and out over time, hoping to bring my presence / attention back to myself frequently. This occured initially with the novelty of the effect, but it wore off quickly as I began straining my eyes to see through myself whilst reading tweets. I adopted a &#8220;look away every 20 seconds approach&#8221; so as to save my eyesight from its inevitable demise, which made for a much slower engagement with the Twitter feed than normal.

As I faded in on the screen, I looked at myself, and I considered that my presense was more &#8220;here&#8221; than &#8220;there&#8221;. Both presences are illusionary, one directly reflecting reality through a camera lens; I took a moment to bring my attention to how I was seeing the screen, through my eyes and noticing how the bridge of my nose is at the edges of my vision.

In summary, this plugin makes Twitter unusable. The source code for the initial experiment can be found <a href="https://gist.github.com/jhancock532/500d0c8b7fe4b1de55e79bdbb79737a8" data-type="URL" data-id="https://gist.github.com/jhancock532/500d0c8b7fe4b1de55e79bdbb79737a8">on GitHub</a>.