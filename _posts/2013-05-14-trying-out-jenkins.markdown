---
layout: post
title: Trying out Jenkins
published: true
categories: [stackato, jenkins]
tags: [continuous integration, stackato]
---

Another "meta" post I'm afraid. That is, I'm blogging for the purpose of trying out something new with stackato. In this case, continuously deploying it to Stackato using Jenkins. Let's see how it goes. :)

I'm basically just making little changes to this particular post, then committing those changes to Github. This in turn triggers a Jenkins build process via the Git plugin which deploys the Jekyll site to Stackato with a unique URL **and** the 'troytest.stacka.to' URL. If you [refresh this page](http://troytest.stacka.to/2013/05/14/trying-out-jenkins/) on the 'troytest.troytop.net' URL, you should see various versions of it at random because each version is added to a load balanced pool.

We'll consider the "production" URL for this blog to be 'troytop.net' (without the 'blog' subdomain) which is set in the Stackato Management Console or with the 'stackato' client. You can likewise add numerous releases into that pool, but it's done manually. 

If you see this line of text, you're looking at build #19 or later.

If you see this line of text, you're looking at build #20 or later.

This line is for build #21, but I'll also be making a possibly breaking change in the deployment config (intentionally), so it may not show up till build #22.

Note: Jenkins regarded build #21 as a succes, but the application actually fails on Stackato because not enough memory has been allocated to successfully run Jekyll. In a real world continuous deployment setup, you would set up tests for this.

Fixing the `mem:` setting for build #22.

Build #23 adds categories, should be no breaking changes.