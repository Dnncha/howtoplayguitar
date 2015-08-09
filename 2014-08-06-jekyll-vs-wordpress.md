---
layout:     post
title:      Jekyll vs Wordpress
date:       2015-08-06 23:00:00
permalink: /jekyll-vs-wordpress
summary:    If you've grown tired of blogging in Wordpress, there's always Jekyll.
categories: jekyll wordpress blogging cms
---

Wordpress is is a truly remarkable package that solves all sorts of problems. It's an all in one publishing system that I can barely believe is free. However, over the years, I've become frustrated with my workflow with it. The network lag while clicking through the dashboard often gets on my nerves when I've had a few coffees. I decided I wanted a blog that I could develop and write locally, and had a one button push up to the server. Ideally I'd write some Markdown in Byword, and then have it automatically converted and pushed to the server.

So what I was looking for, it turns out, was [Jeykll](http://jekyllrb.com/), running on Github pages. It is a static site generator and it keeps your entire blog in a neat little folder, in text files.

##It's easy to get set up

It doesn't take long to get Jekyll set up on GitHub Pages, although I guess it might be a confusing  process if you're not familiar with the command line. 
If you've used Git before, you can get a site up and running on Github Pages in no time. 

Smashing Magazine has [a nice tutorial to get you get Jekyll set up on Github pages.](http://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/).

After you've got that stuff set up, simply grab a theme from [Jekyll themes](http://jekyllthemes.org/) and you're off to the races. 

##Static sites are performant.
Thanks to Github's great infrastructure, and the fact that Jekyll doesn't need to query a database, this site loads up very quickly indeed. If I was running Wordpress on a typical shared host, like [Blacknight](www.blacknight.com) or [Bluehost](www.bluehost.com), I'd have to do a bit of work to get anywhere near a 300ms page load.  

![Jekyll Speed Test]({{ site.url }}/images/jekyll_plus_github_pages_equals_fast.png)

##Markdown is great

Markdown is my preferred method of writing for the web. If you've never heard of it, you can have a look at this [handy markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

I'm writing this post in [Byword](www.byword.com), but you could also write your blog in [Sublime Text](www.sublimetext.com), TextEdit or even [Drafts for iOS](http://agiletortoise.com/drafts/). 

##SEO in Jekyll

Wordpress has Yoast, what does Jekyll have to offer to help you jostle for position in Google? 

###Front Matter
Front Matter lets you easily rewrite your title and meta description, right at the top of your article, in plain text. 

{% highlight yaml %}
---
title:      Jekyll vs Wordpress
date:       2015-08-06 23:00:00
permalink:  /jekyll-vs-wordpress
summary:    If you've grown tired of blogging in Wordpress, there's always Jekyll.
categories: jekyll wordpress blogging cms
---
{% endhighlight %}

If you don't specify a meta description, Jekyll will fall back to your site's default. I think that this is a much more graceful solution than running a hefty SEO plugin for Wordpress that runs ads in your dashboard. 

###"But isn't Yoast more powerful than that?"
Yoast generates sitemaps, which is good, but [Jekyll can do that too](https://help.github.com/articles/sitemaps-for-github-pages/).  It lets you rewrite page titles and meta descriptions, but you can do that with Front Matter. 

Yoast does have that fancy content analysis feature - it asks you to specify a keyword and then advises you to plaster it all over the place in your title, in your description etc. 

With SEO, I've decided to take Matt Cutts' advice and forget about nitty gritty SEO tricks and focus on content. If Google uses, say, 200 factors when it ranks a webpage, how big of an SEO boost does Yoast style keyword stuffing really give you? Is the modern googlebot really convinced by seeing the same phrase in the description and the title? *Perhaps* it's more interested in bounce rates and the amount of time the user stays on the site. Those metrics are harder for webmasters to interfere with, and webmasters can't be trusted not to vote for themselves.