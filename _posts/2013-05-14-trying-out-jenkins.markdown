---
layout: post
title: Trying out Jenkins
published: true
---

Another "meta" post I'm afraid. That is, I'm going to be blogging for the purpose of trying out something new with my blog. In this case, continuously deploying it to Stackato using Jenkins. Let's see how it goes. :)

I'm basically just making little changes to this particular post, then committing those changes to Github. This in turn triggers a Jenkins build process which deploys the Jekyll site to Stackato with a unique URL **and** the blog.troytop.net URL. If you refresh this page using the 'blog.troytop.net' URL, you should see various versions of it at random because each version is added to a load balanced pool.

We'll consider the "production" URL for this blog to be 'troytop.net' (without the 'blog' subdomain) which is set in the Stackato Management Console or with the 'stackato' client. You can likewise add numerous releases into that pool, but it's done manually. 

