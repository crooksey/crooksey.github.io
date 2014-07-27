---
layout: post
title: Why I stopped using Django
description: "The rhymes and reasons behind why I stopped using Django."
modified: 2014-07-21
tags: [django, pyramid, sqlalchemy]
image:
  feature: abstract-10.jpg
comments: true
share: true  
---

This is my own personal opinion, many people love Django, I however am not one of those users.

### Background

I was an avid Django user for at least 18 months, using and contributing to several projects. At first everything was rosy, then I experienced upgrading from 1.25 to 1.3.

When I first started with Django it was more due to the frustration with Ruby on Rails, I had several projects using Spree and Radiant CMS. I had been using Ruby/Rails for around a year, doing fairly small projects, it was great for what I needed, but I never really felt comfortable with it. I  honestly can't remember what versions of Ruby I was using, but I think it was 1.8. I had a spree site, linked to a Radiant CMS, then spree upgraded to Ruby 1.9 and Radiant didn't. To get the new features (and support) of spree, I ended up having to split my site across two applications, this ran for about 6 months, until I had given up fighting, and looked at writing a new platform.

I eventually migrated to python (which I had used in college) and re-wrote my setup for Django. I used the brilliant Django-cms, I wrote a custom application adapted from Arkestra. This was a time when the CMS and Arkestra were both under rapid development, but I loved both projects and even helped contribute.

### The honeymoon period

Everything was great, then django 1.3 became a final release and apps started moving, It wasn't really a problem but I remember migrating from django admin media to static files and various other code changes, not something I really enjoyed. Then everything was fine again, untill 1.4 came out. This whole process really got on my nerves and changing code every version upgrade was a pain, especially when different libraries updated at different paces. Which basically means, if you want to use code that others have written for django, expect to be updating a lot of it as you migrate and projects get left behind.

I ended up re-writing a lot of third party apps, just so I could migrate my CMS to the the latest version.

### And then I needed more

I was then approached to write a custom CRM system for a company, whilst evaluating the best options, I stumbled across Pyramid + SQLAlchemy. It was love at first sight, it was writing pure python with a few web renderers. I could see that major version upgrades wouldn't be a problem, as I was just writing python.

SQLAlchemy is just a god send, words cannot describe how awesome this package is.

Coding with SQLAlchemy and Pyramid feels brilliant after coming from Django, there are literally no limitations, write what you want quickly and easily and knowing that I am not going to have a headache when a new major version comes out, is even better. Its been 18months with Pyramid now and the documentation and the community are brilliant.

If you have a rainy day to have a go with Pyramid, do it. You won't regret it.




