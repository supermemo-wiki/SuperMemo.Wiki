---
title: The future of SuperMemo
description: 
published: true
date: 2020-12-21T13:06:54.234Z
tags: 
editor: markdown
dateCreated: 2020-12-17T22:53:23.617Z
---

In this page I will update features that I think would offer the biggest increase in learning productivity in SM. This list is not fixed and will be updated from time to time.

# #1 Incremental Web Browsing

> This feature is currently implemented with very simple AHK script (and chrome extension) and I hope to see more robust version implemented in SMA or SM in the future.
{.is-warning}


Import function in SM is old news and adds only extra friction to the curious mind. The SM importing can be sped up with external tools. However, even with scripts to speed up importing, there is still a problem of not being able to jump around hyperlinks quickly, lack of formatting in some cases and not being able to utilize the increasing number of interactive tools in websites. SM cannot handle this; it is always more flexible to read in browser. The navigation and jumping around in browser are always superior and the benefits of this is not to be overlooked. When I find a goldmine, I do not want to stop to import the whole page! I might want only two sentences from different locations in the page. I want to read and extract only the greatest golden nuggets to SM! I.e., it will always be more flexible to read (initially) in browser than in SM.

This is the plan: read initially in browser, review and create items in SM.

While it can be argued that the cost of importing is negligible as compared to the value a GOLDEN article offers, this friction is not to be overlooked. In fact, I was big believer of focusing only on the flow of knowledge and ignoring these small costs. When I created the script to extract knowledge directly from web, I did not anticipate it to make a great difference. I was so wrong! 

> To understand the difference incremental web browsing makes to the learning process, you need to try it yourself!
> 
{.is-info}

I made a simple AHK script which allows me to extract things from any website and leaving a highlight on the site, which will remain there even if you shut down your computer (the highlights are saved locally). 

This is done with simple copy paste function (you can ask me for the script in discord, it's too dirty currently to be released) and chrome extension called highlighter https://chrome.google.com/webstore/detail/highlighter/fdfcjfoifbjplmificlkdfneafllkgmn

github for the highlighter: https://github.com/jeromepl/highlighter

![web1.png](/blogs/naess/futureofsm/web1.png)

![web2.png](/blogs/naess/futureofsm/web2.png)

![web3.png](/blogs/naess/futureofsm/web3.png)

## Benefits
This script increased value of my collection by HUGE amount. When I am able to read in browser, I can QUICKLY sift away the garbage, navigate like a ninja and extract pieces from here and there, without importing slowing me down. I am more inclined to extract ONLY the golden nuggets because the sifting through garbage is so fast. In contrast, when I used to import every page to SM, I was more inclined to settle with lower value material, just because benefits of finding better alternative did not overcome the costs of importing. This definitely leads to deterioration in value of the collection as we rarely can predict the impact of exploring and finding only the greatest pieces of knowledge.

> Incremental web browsing takes sifting away the garbage and filling your collection ONLY with the most valuable stuff to the next level!

## Compared to old way of importing

At any given moment, value/sentence ratio of your collection equals total value of the sentences divided by the number of sentences in your collection. When you import a whole wikipedia article and all you want from the article is couple sentences, the value/sentence ratio goes down drastically (a lot of noise added with little value). When you come back to the article later after importing, it might be the case that you can't locate the essential pieces you imported the article for in the first place, so you have to resort to sift through the noise. Worse yet, you might be inclined to start reading from top to down just because SM presents you that article. Value is lost here and unnecessary time spent. This affects the pleasure of learning also.

Proficient SM user can cope with these pitfalls, however they will always slow him down and make the process less fun. For a beginner, the consequences might be worse: there is more noise which he is inclined to create poor items of, he might drown in countless of noisy extracts from the noisy article with only little value realized. This brings the efficiency of SuperMemo down drastically. For beginner forced to import the whole articles (or atleast noisy chunks), pleasure and efficiency of learning decreases significantly.

> The importing functionality of SuperMemo might lead to deterioration of the pleasure of learning and decrease efficiency of the whole learning process

In contrast, with the direct extracting from websites, you are getting only the essentials and not importing the associated noise with these. It's easy to see how this increases value of your collection drastically. Lot of value with no noise whatsoever. 

I'm aware that you could highlight text in IE and import only the highlighted text, however you can't take one sentence from top of the article and one from the bottom (you can only highlight one chunk). On top of that, you need to stop the consumption and extraction of the information to do unnecessary function of importing to SM.

## Functionality
With alt+x you can extract from browser. The selected text will be marked with the highlighter extension. Script will activate SM window and paste the text selected and also link for the website. After that, script will activate browser again

Shift+alt+X pops up prompt which asks for note and/or priority. Same functionality as explained before, but note will be pasted above the highlighted text and priority will be assigned.

Ctrl+alt+Enter will quickly filter the article, when user rather use SM stylesheet determined formatting. 
This sends the following keystrokes: F6 + Ctrl+A + S to apply all but "spacing filter)

# #2 Prioritization framework
> This feature is implemented in AHK but is desirable to be integrated in native SM or SMA. Also in the pre-existing framework (see the youtube video), there is room for improvement.
{.is-warning}

Priorities determined by some framework instead of arbitrary priority ranges. It is easier to prioritize by categories (e.g. applicable / urgent / mildly interesting) than abstract ranges. See: [Youtube: Priority Heuristics in SuperMemo](https://youtu.be/OwV5HPKMrbg) for direction.

# #3 Cloze Hinter
I can't believe this is not natively supported! Alt+shift+Z on highlighted text to pop up prompt for hint.

Result: exemplary cloze with `[...](hint)`

Tons of alt+lefting and navigating saved! Luckily JamesB has created SMA plugin for this, however the prompt is to be improved.

# #4 PDF Notes
Alexis' PDF plugin is revolutionary! However as PDFs (textbooks) are usually full of verbiage, a lot of the time it's better to summarize what you are reading and then IR your summaries. Margin for notes would be super helpful here -> Write notes as you read (in margin of the PDF viewer), extract these notes and process them in SM.