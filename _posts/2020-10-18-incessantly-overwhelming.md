---
id: 157
title: Incessantly Overwhelming
date: 2020-10-18T16:16:55+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=157
permalink: /incessantly-overwhelming/
categories:
  - Web Projects
---
<blockquote class="wp-block-quote">
  <p>
    Listening to people speaking their truth opens up the idea that, ultimately, we all have a similar goal, which is to find an authentic sense of our self in a world that is incessantly overwhelming.
  </p>
  
  <cite><a href="https://www.theguardian.com/tv-and-radio/2020/oct/13/jordan-stephens-mental-health-gentrified">Jordan Stephens, The Guardian</a></cite>
</blockquote>

As I scroll through my Twitter timeline, the series of tweets also slides through my head, being passively played out and filtered as to whether it&#8217;s deserving of engagement. If I was to engage thoughtfully with all the tweets on this timeline, I would quickly become overwhelmed &#8211; with an inbuilt attention filter, I&#8217;m able to passively scroll for much longer. That&#8217;s a theory anyway.

What if we couldn&#8217;t passively scroll through tweets and just forget them as they leave our field of vision? What if all these tweets we read, looked at or watched hung about with us, leaving faint traces in our memory? My next project, `content-aggregation.js`, visualises these traces, leaving the ghost of the tweets you&#8217;ve scrolled past still visible on the timeline.

<!--more--><figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="576" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/webpage-overload-1024x576.png" alt="" class="wp-image-161" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/webpage-overload-1024x576.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/webpage-overload-300x169.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/webpage-overload-768x432.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/webpage-overload-1536x864.png 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/webpage-overload.png 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>Content Aggregation &#8211; The Dark Cloud</figcaption></figure> 

In the first version, I let tweets pile up at the top of the screen, making the viewing of new content still feasible. In the second version, I gave the ghost data free range to haunt the webpage wherever it chooses.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="576" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/even-further-into-the-noise-1024x576.png" alt="" class="wp-image-163" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/even-further-into-the-noise-1024x576.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/even-further-into-the-noise-300x169.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/even-further-into-the-noise-768x432.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/even-further-into-the-noise-1536x864.png 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/even-further-into-the-noise.png 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>Content Aggregation &#8211; So Much Nuance</figcaption></figure> 

After expermenting with taking canvas screenshots, I found it much easier to duplicate the entire tweet HTML and restyle it. The twitter feed container gets new tweets added to it and old tweets removed periodically, so I added an event listener to trigger my code whenever new tweets were appended. [The source code is available on GitHub](https://gist.github.com/jhancock532/64b15a90a82ba184ec9c47f6db4ecf84). There&#8217;s a good reason old tweets are removed from the timeline &#8211; too many tweets and the webpage starts lagging severly. Too much information and our brain doesn&#8217;t fair so well either.

We don&#8217;t operate as machines however. When I&#8217;m overwhelmed, I notice less, perhaps because I already have enough of my attention on other things, or I&#8217;ve got a backlog of information I still need to sort out in my head. I can easily ignore this feeling of being overwhelmed however, especially when I&#8217;ve got a series of enterntaining tweets to read through or the lastest trending topics to check out. The passive distraction of checking Twitter can help me escape my sense of being overwhelmed (oftentimes, you guessed it, from too much internet).

In the above artwork, the ghost tweets eventually cover the screen and we can&#8217;t scroll to view new content anymore. It would be more realistic to have the tweets appear in full opacity; as you scroll, you can still see the new tweets appear as much as you like, but the old content and the webpage itself gets obscured and forgotten.<figure class="wp-block-image size-large">

<img loading="lazy" width="1024" height="576" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/disparate-content-1024x576.png" alt="" class="wp-image-165" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/disparate-content-1024x576.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/disparate-content-300x169.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/disparate-content-768x432.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/disparate-content-1536x864.png 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/disparate-content.png 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> <figcaption>Content Aggregation &#8211; Of A Disparate Nature</figcaption></figure> 

In this case, I like how having the tweets pop up all over the screen really highlights how unrelated they are to each other. I was aimlessly scrolling through this for a while, not reading the content much, just seeing the effect it creates. There was a weird period whilst scrolling where I only saw tweets liked by a handful of Twitter users (eg Nancy Wood). I wonder if Twitter picked up on the weird fast scrolling behaviour and adjusted the content it gave me accordingly.

I recorded a video of me scrolling through it all. As content is often so quick to be discarded after we see it for the first time, I forced myself to watch through the video again. I felt emotional revulsion towards doing this. I stopped watching five minutes and 50 seconds in, as it was too much. I didn&#8217;t have control over how fast the data was coming in, and the data had no novelty to distract me, so I felt a lot more overwhelmed. Good experiment!

Here&#8217;s the video if you&#8217;re interested.