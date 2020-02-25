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
Let me also say that I am not here to argue how *you* define **serverless** 
or whether *you* think it's an inappropriate, unfortunate, or misleading moniker.

Let's get that straight from the jump, Spanky.

Now when I think of serverless, three things come to mind:

    1. Little to no server management.
    2. High availability and scalability.
    3. Lower costs.

So when it came to my first ***ever*** blog, the overall theme of which is about going serverless, 
I couldn't very well spin up a blog using the classic web server model, now could I?

No, I needed to find a way to host my blog in a static, low cost way. 
I also needed a way of doing so that allowed visitors to search the blog and leave comments if so desired.

Sounds easy, right?

Wait a minute, Spanky. You don't know the first thing about spinning up a blog, let alone a serverless one. 
Where to start? What to do? Well, do what you always do when faced with a technology you don't know: 
*Jump right in and start researching*.

Googling "static blogs with search and comments capability" led me to [Jekyll](https://jekyllrb.com/) 
and [GitHub Pages](https://pages.github.com/). Within a matter of hours, 
I was able to get a comprehensive overview of these technologies 
and publish a working blog template to a custom domain with an SSL to boot (thank you, Google Domains).

And you know the best part? ***Absolutely free!***

That's right, Spanky.

What about search and comments capability? That turned out to be just as easy as well, 
and did not compromise my serverless goals.

For search, I came across this [article](https://learn.cloudcannon.com/jekyll/jekyll-search-using-lunr-js/) 
on [cloudcannon](https://learn.cloudcannon.com/) using this technology [Lunr](https://lunrjs.com/). 
Basically, this is a super simple (to use) JavaScript plugin that can run client-side (i.e., in browser). 
With the article's help, I quickly implemented a nice way for users to search all the blog posts.

Cost? ***Absolutely free!***

Finally, for comments, I came across this Jekyll plugin [utterances](https://utteranc.es/) developed by 
Microsoft alum [Jeremy Danyow](https://github.com/jdanyow/). This is a GitHub App that uses your repo's GitHub 
issues feature to create and store user comments by matching the comments to a particular blog post via some factor that you 
predetermine (such as, the title of the post). 

Yeah, someone who wishes to leave a comment has to have a GitHub account and be signed in, 
so this wouldn't make sense for a non-tech blog, where most of the visitors are likely to have never heard of GitHub. 
But for *this* blog it's more than adequate...and secure. And as you can see below, it's super sweet!

Cost? ***Absolutely free!***

Now, let's reexamine whether my new blog meets my serverless goals:

    1. Little to no server management.

:+1: No server had to be spun up or provisioned. No scale-up or scale-out settings had to be tweaked or messed with.

    2. High availability and scalability.

:+1: Well...sort of. GitHub Pages does have some 
[limitations](https://help.github.com/en/github/working-with-github-pages/about-github-pages#guidelines-for-using-github-pages). 
But if my blog grew and became highly popular, I could always drop a CDN in front or move it elsewhere (Azure Storage).
    
    3. Lower costs.

:+1: ***Absolutely free!*** (I should point out that the custom domain costs $12 a year, but who's counting three cents a day? 
Also, you more than welcome to stick with the https-protected domain that GitHub Pages give you for free out of the box.)

Well, there you have it. First post on my serverless blog in the books. You can view the source code for this blog 
[here](https://github.com/allan-mobley-jr/hucklepuck/). Feel free to clone, download, or fork the repo. Hope to see you next time!