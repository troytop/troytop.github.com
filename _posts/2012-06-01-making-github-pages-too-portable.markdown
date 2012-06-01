---
layout: post
title: Making Github Pages Too Portable
published: true
---

So, after a significant delay, I'm back on the Jekyll/Github Pages wagon. I've successfully [stolen some style](https://github.com/dueyfinster/dueyfinster.github.com/), set up a CNAME, set up Disqus, and put my mug on the front page. Now that I've got this far, I have to ask myself: Why did I think blogging on Github Pages would be a good idea?

Ah right, portability.

Blogging with a static site generator is indeed portable. I've been able to move this one around to various Stackato systems by just adding a config file, and it could also be made to work on Cloud Foundry (haven't tried yet) or Heroku (using pretty much the [same buildpack](https://github.com/troytop/stackato-buildpack-jekyll) I used for Stackato).

Great! I can move my blog pretty much anywhere I want, as long as it can run Jekyll or some compatible engine.

And so can you!

No, really. You could go ahead and grab this whole site and spin it up anywhere you want, which makes me wonder why [sploggers](http://en.wikipedia.org/wiki/Spam_blog) haven't taken advantage of this already.

There are a number very technically literate people I know who are using Github Pages for their personal blogs. Unlike this blog, they've accrued a great deal of valuable technical advice and insights - great material for the budding blog scraper. They wouldn't even have to scrape content from RSS, just clone the repo and inject some ads.

I haven't actually seen this phenomenon in the wild yet, so I'm not overly concerned. I suppose it all leads back to one of the [fundamental problem of identity on the net](http://en.wikipedia.org/wiki/On_the_Internet,_nobody_knows_you%27re_a_dog). Could you ever really know if this is the blog of one Troy Topnik, Technical Writer, or just some guy who cloned my public Github repo?


