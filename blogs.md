---
title: User Blogs
description: Index of SuperMemo.wiki user blogs.
published: true
date: 2020-12-18T15:14:16.669Z
tags: 
editor: markdown
dateCreated: 2020-12-17T22:28:40.321Z
---

This is an index of SuperMemo.wiki **user blogs**.

> Content published in user blogs does not reflect the views of SuperMemo.wiki or SuperMemo World.
{.is-warning}

# Creating a blog

If you are interested in having your personal page on this wiki, you can follow the procedure below.

## Content policy

Please exercise judgement when publishing content on your user page. This is a wiki about SuperMemo, learning and personal progress.

Offensive or inappropriate content (e.g. idealogical propaganda) will be removed.

## Creating pages

1. Create a new page underneath `/blogs/[username]`,
2. If you want to create more than a single page, create additionals pages under `/blogs/[username]/[page-title]` (e.g. `/blogs/alexis/why-I-love-learning`.

```kroki
blockdiag

{
  span_width = 128;  // default value is 64
  
	blogs [label = "Blogs", color = "greenyellow"];
  
  b-alexis [label = "Alexis' Man Cave"];
  b-naess [label = "Naess' Corner"];
  b-dots [shape = "dots"];
  b-users [label ="Other users"]
  
  b-a-page1[label = "How I Learned To Stop Worrying And Love Learning", width = 192];
  b-a-page2[label = "Theory of the traditional French baguette", width = 192];
  
  blogs -> b-naess [label="/naess"]
  blogs -> b-alexis [label="/alexis"]
  blogs -> b-dots [style = "none"];
  blogs -> b-users
  
           b-alexis -> b-a-page1 [label="/why-I-love-learning"]
           b-alexis -> b-a-page2 [label="/theory-of-the-French-baguette"]
}
```

## Requesting a subdomain

If you want to have your own subdomain such as https://alexis.supermemo.wiki/, send an email by clicking on the link below. Make sure that you:
1. Have created an account on this wiki,
2. Have created a page for your blog on this wiki,
3. Include your username, and the link to your wiki page in the request.

- [Request a subdomain *Request by email, please include your wiki username and page.*](mailto:alexis@supermemo.wiki?subject=[SuperMemo.wiki]%20I%20would%20like%20to%20create%20a%20blog&body=Hello,%0D%0A%0D%0ACould%20you%20please%20create%20a%20subdomain%20for%20my%20blog?%20My%20username%20is%20[username].%20My%20wiki%20page%20is%20[https://www.supermemo.wiki/blogs/[username].%0D%0A%0D%0AThanks!)
{.links-list}

# User blogs

- [Naess' Corner *The wacky journey of a well-schooled student.*](https://naess.supermemo.wiki/)
- [Alexis Incogito *Work in progress.*](https://alexis.supermemo.wiki/)
- [Guillem's Corner *Non-descriptive generic text*](https://guillem.supermemo.wiki)
- [Maths' Corner *Non-descriptive generic text*](https://maths.supermemo.wiki)
- [Gilgamesh's Corner *Non-descriptive generic text*](https://gilgamesh.supermemo.wiki)
{.links-list}
