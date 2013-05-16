---
layout: post
title: Trying out Jenkins
published: true
---

Another "meta" post I'm afraid. That is, I'm going to be blogging for the purpose of trying out something new with my blog. In this case, continuously deploying it to Stackato using Jenkins. Let's see how it goes. :)

I'm basically just making little changes to this particular post, then committing those changes to Github. This in turn triggers a Jenkins build process which deploys the Jekyll site to Stackato with a unique URL **and** the default troytop.net URL. If you refresh this page, you should see various versions of it at random because each version is added to a load balanced pool.
