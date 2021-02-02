---
project: Web Tech
title: Web 2.0 Disruptions
date: 2020-10-07T13:29:57+00:00
author: James
layout: post
guid: https://jhancock532.github.io/blog/?p=63
permalink: /web-2-0-disruptions/
tags:
  - Reading
---
<blockquote class="wp-block-quote">
  <p>
    &#8220;The internet just feels like this giant mall, there&#8217;s gotta be more to it&#8221;
  </p>
  
  <cite>Tech Critic on <a href="https://www.thesocialdilemma.com/">The Social Dilemma</a>, a Netflix documentary about how Netflix is ruining our lives.</cite>
</blockquote>

From the previous blog post&#8230; &#8220;Could we create art through deliberately setting context in exaggerated forms, so that the content is percieved in a new light?&#8221; A simple way of doing this is to modify the web browser DOM with some extra CSS styling. You can copy and paste the following code into your browser JavaScript debugger to create a range of striking effects.

<!--more-->

<code>//Rotates all webpage elements randomly.
let elements = document.getElementsByTagName("*");
for (let i = 0; i &lt; elements.length; i++) {
  let randomNumber = (Math.random()*60 - 30).toString();
  elements&#91;i].style.transform = "rotate(" + randomNumber + "deg)";
}</code>

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/incredible-1024x576.png" alt="" class="wp-image-138" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/incredible-1024x576.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/incredible-300x169.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/incredible-768x432.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/incredible-1536x864.png 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/incredible.png 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />
Twitter, Tilted

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/huh-1024x576.png" alt="" class="wp-image-135" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/huh-1024x576.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/huh-300x169.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/huh-768x432.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/huh-1536x864.png 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/huh.png 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" />
Twitter, Colourised

I&#8217;m having a go at creating a web browser extension to apply these effects automatically on visiting a website. As we make a mess of the Twitter brand, our attention is brought to the invisible gallery that the Web 2.0 exists within. The forms of content distribution, once we become familiar to their patterns of scrolling and clicking, are lost as the background of the endless stream of content and information passing through. This doesn&#8217;t have to be the case however; here&#8217;s a more theoretical collection of CodePen demos where form is more important than content.

## Web 2.0 Dependencies

This CodePen demo displays the wrapper code that normally holds the CodePen demo. There is no source code visible in the demo itself.

<p class="codepen" data-height="422" data-theme-id="dark" data-default-tab="result" data-user="jhancock532" data-slug-hash="gOMpVXZ" style="height: 422px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Web 2.0 Dependencies">
  <span>See the Pen <a href="https://codepen.io/jhancock532/pen/gOMpVXZ"> Web 2.0 Dependencies</a> by James Hancock (<a href="https://codepen.io/jhancock532">@jhancock532</a>) on <a href="https://codepen.io">CodePen</a>.</span>
</p>

When viewed in different contexts and by different browser agents, different code is logged into the `<textarea>`. This makes me think of how digital art is always performed&#8230;

<blockquote class="wp-block-quote">
  <p>
    &#8220;<em>The visualisation of digital data is always an act of interpretation by the internet user”</em>
  </p>
  
  <cite>Groys 2016, pp.142–146</cite>
</blockquote>

Groys goes on to explan that the data file is the art, and each web browser performs it in a different way. 

In this case, the performance of the file, the framework for hosting and displaying data provided by CodePen, makes up the majority of the art itself, just as [Alpha](https://superrare.co/artwork-v2/alpha-7713) displays the surrounding context and community within which it exists ([Hazmus, 2020](https://beta.cent.co/Hazmus/+yeln0j)). 

## Web 2.0 Performance

This demo infinitely recurses, an embed embedded in an embed. There is nothing but form.

<p class="codepen" data-height="265" data-theme-id="dark" data-default-tab="result" data-user="jhancock532" data-slug-hash="WNxQzJy" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Web 2.0 Performance">
  <span>See the Pen <a href="https://codepen.io/jhancock532/pen/WNxQzJy"> Web 2.0 Performance</a> by James Hancock (<a href="https://codepen.io/jhancock532">@jhancock532</a>) on <a href="https://codepen.io">CodePen</a>.</span>
</p>

### Abusing Customisations Allowed by Web 2.0

Push the limits of the system with [a 50 character long YouTube channel name](https://www.youtube.com/watch?v=GhtJnFfj_3Y), or just dump <a href="http://animalswithinanimals.com/generator/generator.html" data-type="URL" data-id="http://animalswithinanimals.com/generator/generator.html">a mess of glitch text</a> into the text submission box. Try using [qwerty.dev](https://qwerty.dev/fancy-font-generator/) to play with a range of 🅕🅐🅝🅒🅨 𝕗𝕠𝕟𝕥 tools.

We&#8217;re dancing within the constraints of the system, trying to push and break the brand limitations, the dictatorship of the brand asthetic. Surprisingly, CodePen is remarkably open to users doing this. You can customise the CSS of your [profile page](https://codepen.io/jhancock532/) extensively&#8230;

<img loading="lazy" src="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/image-1024x576.png" alt="" class="wp-image-107" srcset="https://jhancock532.github.io/blog/wp-content/uploads/2020/10/image-1024x576.png 1024w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/image-300x169.png 300w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/image-768x432.png 768w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/image-1536x864.png 1536w, https://jhancock532.github.io/blog/wp-content/uploads/2020/10/image.png 1920w" sizes="(max-width: 767px) 89vw, (max-width: 1000px) 54vw, (max-width: 1071px) 543px, 580px" /> 

You&#8217;ll notice that I have 45, 179 followers. We trust Twitter and Instagram to report the number of followers of each account accurately. However, on CodePen, you also have to trust and verfiy that I haven&#8217;t modified this number with my custom CSS styling. If you&#8217;re unaware that the option for custom styling exists you might be easily misled.

To do this for yourself, [fork my source code](https://codepen.io/jhancock532/pen/ExyVYxQ) then include a link to your forked pen on the profile settings page. 

#### References

Groys, B., 2016. In The Flow. 2nd ed. London: Verso, p.1.