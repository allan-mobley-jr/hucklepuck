---
layout: post
comments: true
title: Blog Building
---
Before we get to the overall topic of *The Hucklepuck*,
which concerns moving a monolithic enterprise application to a serverless one, 
I thought I would use the first post to chronicle 
how I built this blog with that very serverless theme in mind.

Let me start off by saying that I am by no means an expert on going serverless. 
Let me also say that I am not here to argue how *you* define the term 
or whether *you* think it's an appropriate, unfortunate, or misleading moniker.

Let's get that straight from the jump.

Now when I think of serverless, three things come to mind:

    1. Little to no server management.
    2. High availability and scalability.
    3. Lower costs.

So when it came to my first ***ever*** blog, the overall theme of which is about going serverless, 
I couldn't very well spin up a blog using the classic web server model. 
That would be hypocritical to say the least.

No, I needed to find a way to host my blog in a static, low cost way. 
I also needed a way of doing so that allowed visitors to search the blog and leave comments if so desired. 
Sounds easy, right?

Wait a minute, Spanky. I did not know the first thing about spinning up a blog, let alone a serverless one. 
Where should I start? What should I do? 
Well, I did what I always do when faced with a technology I don't know: 
*I jump right in and start researching*.

Googling "static blogs with search and comment capability" led me to [Jekyll](https://jekyllrb.com/) 
and [GitHub Pages](https://pages.github.com/). Within a matter of hours, 
I was able to get a comprehensive overview of these technologies 
and publish a working blog template to a custom domain with an SSL to boot.

No server had to be spun up or provisioned. No scale up or scale out settings had to be tweaked. 
And you know the best part? ***Absolutely free!***

That's right, Spanky.