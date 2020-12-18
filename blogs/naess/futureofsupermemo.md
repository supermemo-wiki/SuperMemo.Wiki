---
title: The future of SuperMemo
description: 
published: true
date: 2020-12-18T15:04:10.806Z
tags: 
editor: markdown
dateCreated: 2020-12-17T22:53:23.617Z
---

In this page I will update features that I think would offer the biggest increase in learning productivity in SM. This list is not fixed and will be updated from time to time.

# #1 Incremental Web Browsing

> This feature is currently implemented with very simple AHK script (and chrome extension) and I hope to see more robust version implemented in SMA or SM in the future.
{.is-warning}


Import function in SM is old news and adds only extra friction for curious mind. The SM importing can be sped up with external tools. However, even with scripts to speed up importing, there is still a problem of not being able to jump around hyperlinks quickly, lack of formatting in some cases and not being able to utilize the increasing amount of interactive tools in websites. SM can not handle this, it is always more flexible to read in browser. The navigation and jumping around in browser is always superior and the benefits of this is not to be overlooked. When I find a goldmine, I do not want to stop to import the whole page! I might want only two sentences from different locations in the page. I want to read and extract only the greatest golden nuggets to SM! I.e. it will always be more flexible to read in browser than in SM.

While it can be argued that the cost of importing is neglible as compared to the value a GOLDEN articles offers, this friction is not to be overlooked. In fact, I was big believer of focusing only on the flow of knowledge and ignoring these small costs. When I created the script to extract knowledge directly from web, I did not anticipate it to make a great difference. I was so wrong! 

> To understand the difference incremental web browsing makes to the learning process, you need to try it yourself!
> 
{.is-info}

I made a simple AHK script which allows me to extract things from any website and leaving a highlight on the site, which will remain there even if you shut down your computer (the highlights are saved locally). 

This is done with simple copy paste function (you can ask me for the script in discord, it's too dirty currently to be released) and chrome extension called highlighter https://chrome.google.com/webstore/detail/highlighter/fdfcjfoifbjplmificlkdfneafllkgmn

github for the highlighter: https://github.com/jeromepl/highlighter

![web1.png](/web1.png)

![web2.png](/web2.png)

![web3.png](/web3.png)

## Benefits
This script increased value of my collection by HUGE amount. When I am able to read in browser, I can QUICKLY sift away the garbage, navigate like a ninja and extract pieces from here and there, without importing slowing me down. I am more inclined to extract ONLY the golden nuggets because the sifting through garbage is so fast. In contrast, when I used to import every page to SM, I was more inclined to settle with lower value material, just because benefits of finding better alternative did not overcome the costs of importing. This definitely leads to deterioration in value of the collection as we rarely can predict the impact of exploring and finding only the greatest pieces of knowledge.

> Incremental web browsing takes sifting away the garbage and filling your collection ONLY with the most valuable stuff to the next level!

## Functionality
With alt+x you can extract from browser. The selected text will be marked with the highlighter extension. Script will activate SM window and paste the text selected and also link for the website. After that, script will activate browser again

Shift+alt+X pops up prompt which asks for note and/or priority. Same functionality as explained before, but note will be pasted above the highlighted text and priority will be assigned.

Ctrl+alt+Enter will quickly filter (F6 + Ctrl+A + S to apply all but "spacing filter) the article, when user rather use SM stylesheet determined formatting.

# #2 Prioritization framework
Priorities determined by some framework instead of arbitrary priority ranges. It is easier to prioritize by categories (e.g. applicable / urgent / mildly interesting) than abstract ranges. See: [Youtube: Priority Heuristics in SuperMemo](https://youtu.be/OwV5HPKMrbg) for direction.
