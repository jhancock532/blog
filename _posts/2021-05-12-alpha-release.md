---
title: Alpha Release
project: Network Practices
date: 2021-02-02T14:42:39+00:00
author: James
layout: post
permalink: /alpha-release/
tags:
  - Reflective Writing
  - Web Projects
---

I've brought the project online with Cloudflare Pages. I attempted to use Netlify, but those guys charge when people get interested in your work. This is a low cost operation, so thank you Cloudflare for the free hosting and HTTPS and DDOS protection. The website demo is now live at [https://fingerprint.garden](https://fingerprint.garden).

I did some early alpha testing - it turns out mobile devices don't support double taps :/ I've added an alternative using Tocca.js, but I don't have any easy way to test this. I hope it works. Alpha testing also revealed that the side of the platform was a valid walkable object, allowing participants to clip through the floor (thanks T for discovering that one!). I've since added a border.

Having actually made and released the website, some artistic merit of the piece becomes apparent to me. This is about what we leave behind; our trail of fingerprints scattered across the web, and what they become.

Time to fix the super dodgy rotation mechanics, then start work on the frontend. Quaternions added, I've used my own gist for this one. Super handy little bit of code - https://gist.github.com/jhancock532/cea8ce753617bd704fb4ac2f5390bc91

This website isn't a fully developed artwork yet. I think it might help if I added a few security cameras that track the garden visitors. Fingerprints are used track users online, so while websites can be a lovely space, it's important to remember that there could be security cameras watching you in the corner, and they know where you've been, and even possibly who you are. (They could even be watching your cursor, for example with hotjar.js)

The visitor has no agency here. They exist in the context of the server to be watched, logged and processed externally. The only actions you have are sitting and walking. Strangely, it is impossible to rest here. The security cameras have become a part of our environment online; perhaps they were embedded into the nature of our online existence from the very beginning; every request and IP address logged... the materiality of the web is evidenced in its logs.

I'll add a render target from the camera object to the screen, maybe pass post-processing over it to make it look security camera like. Add some bold text - "YOU ARE BEING WATCHED" above it? It might be nicer to add text that says "YOU ARE BEING FOLLOWED" because that plays off social media 2.0. I think I better add a heart symbol at the end and cursive text to help it fit the theme... We don't need all caps, because we are complying quite happily with being tracked. This is a positive relationship we've been having for some time with the advertisers, we just haven't realised how good it is.

The juxtaposition of a nice garden and the server observer "stalking" you is bold enough to make the website interesting. I think I'd have to use a really happy font, like Comic Sans, just to get the point across. If it's slightly condesencing that would be even better.

There should be four cameras distributed about the space, because the distribution of watching occurs across many websites (as fun as it is to create one massive tower of security cameras, which could represent a central server).

The video texture / render target loads within the scene well, and I've even made a basic zoom in feature when the person walks away from the camera (via the FOV function, not yet scaled to a linear zoom though). Now it's time to add the camera towers, camera bases, and camera model to the scene. I've made my own security camera in Blender as I couldn't find a nice one online.

Camera models loaded in with towers. Added a seperate camera tower class within the garden class - this is a dodgy way of doing things, as stuff is nested but not directly attached to the cctv camera observer. I have to do this attachment manually :/

Even when you were alone, we were following you.
For all the time you spent watching, we were watching you.
To fall in love the algorithm; never judgemental, always with you.

## The cult of distraction

I introduce you to the cult of distraction. This cult pervades everywhere; we are often simply too distracted to notice it.

Distraction isn't necessarily creation of fantasy; storytelling exists within the bounds of existing knowledge, so no new fantasy is created? Stories retold don't add much fantasy, but new stories, fresh content, do add fresh fantasy?

The cult of distraction is meaningful; it is what makes us human.

What exactly are we being distracted from? Because after all, our conscious attention is limited to one focus at a time! Perhaps we should be expanding our attention to cover more of our selves and surroundings, as practiced in silent meditation? Are we being distracted by our focus? Are we distracted from the immediate presence of reality? But how do you capture or define "the immediate presence of reality" if it is the entirity of our experience? So how do you know when you are distracted, or really percieving all of that what is there? We can conclude that there is no difference, that what we see is all there is, because for that moment, that direction of attention, that was ALL there was. Maybe sometimes broader awareness, maybe less. 

Maybe if we were totally aware of every input, where no input was clouded by thought, we'd even lose the illusionary concepts of self and perception - we'd lose the perception of percieving, then there'd be nothing to percieve. 

Gate, Gate, Paragate, Parasamgate, Bodhi Svaha.

Distraction is attention and both are illusion; an illusion that is real, for as real as reality is.

**I AM NOTHING IF NOT LITERAL-MINDED. TRICKERY WITH WORDS IS WHERE *HUMANS* LIVE.**
'All right,' said Susan. 'I'm not stupid. You're saying that humans need ... *fantasies* to make life bearable.'
**REALLY? AS IF IT WAS SOME KIND OF PINK PILL? NO. HUMANS NEED FANTASY TO BE HUMAN. TO BE THE PLACE WHERE THE FALLING ANGEL MEETS THE RISING APE.**
'Tooth fairies? Hogfathers? Little-'
**YES. AS PRACTICE. YOU HAVE TO START OUT LEARNING TO BELIEVE THE *LITTLE* LIES.**
'So we can believe the big ones?'
**YES. JUSTICE. MERCY. DUTY. THAT SORT OF THING.**
'They're not the same at all!'
**YOU THINK SO? THEN TAKE THE UNIVERSE AND GRIND IT DOWN TO THE FINEST POWDER AND SIEVE IT THROUGH THE FINEST SIEVE AND THEN *SHOW* ME ONE ATOM OF JUSTICE, ONE MOLECULE OF MERCY. AND YET -** Death waved a hand. **AND YET YOU ACT AS IF THERE IS SOME IDEAL ORDER IN THE WORLD, AS IF THERE IS SOME ... SOME *RIGHTNESS* IN THE UNIVERSE BY WHICH IT MAY BE JUDGED.**
'Yes, but people have *got* to believe that, or what's the *point*-'
**MY POINT EXACTLY.**

Hogfather, Terry Pratchett - Page 422, 423

Distraction, fantasy and symbol entwine in toxic and productive relationships. The internet is an excellent microcosm of all 
The internet aids the forming these fantasies that make us human

An infinite series of distractions is presented on Twitter, Facebook, TikTok, Instagram, YouTube, Reddit.

Saying goodbye to yourself, as you once were.

I watch a Twitch streamer diagnosed with ADHD down caffiene to broadcast a stream after her day job  editing videos. The chat rallies around her, excited to be here, being part of something bigger. A few of her tiktoks have gone viral recently, the steamer effuses her praise and thanks of the community. This wholesome mutual support builds my investment in her character, I am delighted to see a person I like succeed, a person who I feel is deserving of success. A person reduced to a story, a story played out in our highest fantasy, reality.

But not all stories are helpful; some stories are toxic, leading to self hatred, needless anxiety, illusionary imaginings of control. It is good to critique and question the stories that cause us hurt - stories about what or who we should be, or how we should act. It is also vital to remember that underneath the stories we tell, a creature is living.