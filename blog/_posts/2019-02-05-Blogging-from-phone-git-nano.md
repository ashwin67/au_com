---
layout: post
title: Blogging from my phone with Git and Nano
date: 2019-02-05
img: thumbnails/how_to_blog_small.png
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- New
---

TL;DR
This post is about how I write my blog posts using markdown, push it to bitbucket, automatically build the code using circleci (resulting in static html pages) and push the result to firebase resulting in the page you are seeing now.

![Process](/assets/code/how_to_blog.png "jekyll markdown - bitbucket - circleci - firebase - blog")

Summary: To setup the above chain, I used a laptop without which debugging would have been a pain. Once past the setup phase, I am able to now create a new text file on my phone, write some contents and push it to my bitbucket repository. CircleCI then gets this push notification and immediately builds it. The source in the repository is based on Jekyll. CircleCI builds this source and creates html pages out of this. CircleCI then deploys the built html files to firebase resulting in a site like this.

I am not going to rewrite the whole process 
again, so I will just point to this good blog I 
referred to: [https://chris.banes.me/2017/06/02/jekyll-firebase/]
There are some differences you need to take care though. One of the biggest differences is that circleCI is now version 2.0 and hence the configuration needs to be different. Following is my configuration: [Gist Yml configuration](https://gist.github.com/ashwin67/76065e3f95d187b03290bb36f387e3f2).
Probably this configuration could be optimized further to cache some things and run the build faster. One important aspect to note when running the jobs in circleCI is that each of the jobs is independent and data is not shared between them unless you do it specifically. My configuration above takes care of that.

Once you have this working, push to deploy from android becomes quite easy. You just have to install a terminal such as [termux](https://wiki.termux.com/wiki/Main_Page) on your phone. Then install ssh, git and some editor such as nano and you have all that you need. Then write a post in the jekyll posts folder and push it to your repo through the terminal and see it deploy automatically.
