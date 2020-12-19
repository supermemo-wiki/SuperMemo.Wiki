---
title: Creating a Blog
description: 
published: true
date: 2020-12-19T17:34:59.672Z
tags: 
editor: markdown
dateCreated: 2020-12-19T16:59:52.998Z
---

> Please **carefully read the instructions** on this page before creating your personal page.
> 
> Disregarding the policies established here, or abusing the wiki will result in a **permanent ban**.
{.is-warning}

# Content policy

Please **exercise judgement** when publishing content on your user page. This is a wiki about:
- SuperMemo,
- Learning,
- Personal progress.

Offensive or inappropriate content (e.g. idealogical propaganda) will be removed.

# Writing your blog

To create your personal page on the wiki, simply follow the steps below.

## Creating pages

1. Create a new page underneath `/blogs/[username]`,
2. If you want to create more than a single page, create additionals pages under `/blogs/[username]/[page-title]` (e.g. `/blogs/alexis/why-I-love-learning`).

```kroki
blockdiag

{
  span_width = 128;  // default value is 64
  
	blogs [label = "Blogs", color = "greenyellow"];
  
  b-alexis [label = "Alexis' Man Cave"];
  b-naess [label = "Naess' Corner"];
  b-dots [shape = "dots"];
  b-users [label ="Other users"]
  
  b-a-page1[label = "How I Learned To Stop Worrying And Love Learning", width = 200];
  b-a-page2[label = "Theory of the traditional French baguette", width = 200];
  
  blogs -> b-alexis [label="/alexis"];
  
  group first_group {
    // Set group-label
    label = "Alexis' blog sub-pages";

    // Set background-color to this group.
    color = "#77FF77";
    
           b-alexis -> b-a-page1 [label="/why-I-love-learning"];
           b-alexis -> b-a-page2 [label="/theory-of-the-French-baguette"];
  }
  
  blogs -> b-naess [label="/naess"];
  blogs -> b-dots [style = "none"];
  blogs -> b-users;
}
```

### Creating your first page: Step 1

Make sure that the page is located under `/blogs/`. Replace `username` with your pen name.

![Creating a blog step 1](/blogs/blogs-creation-1.png)

### Creating your first page: Step 2

Select <kbd>From Template</kbd> to bootstrap your page with the default settings (markdown), or alternatively select a custom editor.

![Creating a blog step 2](/blogs/blogs-creation-2.png)

### Creating your first page: Step 3

**If you have selected <kbd>From Template</kbd>, select **Blog Template** from the **User Blogs** folder.

![Creating a blog step 3](/blogs/blogs-creation-3.png)

## Editing your page's properties

After creating a page, start editing it and click on the <kbd>Page</kbd> button at the top right of the window.

You can adjust the properties of the current page here. For more details, see:

- [![wikijs.svg](/shared/icons/wikijs.svg =x20){.align-middle} Documentation *Wiki.js page editing documentation.*](https://docs.requarks.io/guide/pages)
{.links-list}

![wikijs-page-properties.png](/shared/wikijs/wikijs-page-properties.png)

## Adding images

> ⚠ _**Please respect the following instructions when adding images and media content**_ ⚠
{.is-warning}

1. All your personal files should be placed under the `/blogs/[username]/` folder,
2. The wiki is not a cloud provider, don't upload large files (e.g. larger than 2MB).

![blogs-media-folder-1.png](/blogs/blogs-media-folder-1.png)

![blogs-media-folder-2.png](/blogs/blogs-media-folder-2.png)

![blogs-media-folder-2.png](/blogs/blogs-media-folder-3.png)

## Formatting guides

[Wiki.js](https://wiki.js.org/) supports several types of **text editors**. The most common format is *Markdown*. The list below will teach you how to leverage the full power of the wiki.

Another great to learn about this wiki's syntax is to look at the source code of other pages.

- [<span style="color:black;" class="mdi mdi-pencil-outline mr-1"></span> Wiki Format *Wiki.js documentation for text editing (markdown, graphs, etc.).*](https://docs.requarks.io/editors)
- [<span style="color:black;" class="mdi mdi-language-markdown mr-1"></span> Markdown *General guide to writing in Markdown.*](https://www.markdownguide.org/)
- [<span style="color:black;" class="mdi mdi-table mr-1"></span> Table generator *Markdown table code generator.*](https://www.tablesgenerator.com/markdown_tables)
{.links-list}

# Requesting a subdomain

If you want to have your own subdomain such as https://alexis.supermemo.wiki/, send an email by clicking on the link below. Make sure that you:
1. Have created an account on this wiki,
2. Have created a page for your blog on this wiki,
3. Include your username, and the link to your wiki page in the request.

- [Request a subdomain *Request by email, please include your wiki username and page.*](mailto:alexis@supermemo.wiki?subject=[SuperMemo.wiki]%20I%20would%20like%20to%20create%20a%20blog&body=Hello,%0D%0A%0D%0ACould%20you%20please%20create%20a%20subdomain%20for%20my%20blog?%20My%20username%20is%20[username].%20My%20wiki%20page%20is%20[https://www.supermemo.wiki/blogs/[username].%0D%0A%0D%0AThanks!)
{.links-list}
