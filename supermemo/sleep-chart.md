---
title: SuperMemo Sleep Chart
description: A simplified version of the official SuperMemo Sleep Chart manual.
published: true
date: 2021-07-13T00:07:08.681Z
tags: 
editor: markdown
dateCreated: 2021-07-01T20:09:30.684Z
---

> Please keep in mind that this page is a work-in-progress. When this banner vanishes, you'll know this article is done. Follow the steps indicated [here](https://www.supermemo.wiki/en/home#editing-this-wiki) if you would like to contribute. Thank you!
{.is-warning}

# Sleep Chart
Sleep Chart is a feature that come with the SuperMemo software. As the name indicates, it is used to record your sleep.

This guide is a simplified version of the official [manual](https://help.supermemo.org/wiki/Sleep_Chart).

# Who is it for?
Sleep Chart is for anyone who has ever searched up online or thought about something along the lines of:
- When is the best time for studying?
- When should I go to bed?
- When should I wake up?
- Should I take a nap? If so, when?

To answer these questions as accurately as possible, the user must have sufficient data.

Furthermore, please take time to read the following disclaimer from the official manual, written by [Dr Piotr Wozniak](https://www.supermemo.wiki/en/supermemo/piotr-wozniak):
> **Important!** Your natural instinct should always take precedence over mathematical models. Moreover, best results in sleep optimization are accomplished in free-running sleep. If you use an alarm clock, or force yourself awake through the night, or take sleeping pills, the models may not adequately account for the chaotic change that is occurring in your sleep control systems.
{.is-info}

# How to access it
Accessing Sleep Chart can be done via three methods:
1. Press the <kbd>F12</kbd> button on your keyboard
2. Press <kbd>Ctrl</kbd>+<kbd>Enter</kbd> which will bring up SuperMemo Commander. Then begin to type in the word "sleep chart" until you see it appear on the menu. Once it appears, press <kbd>Enter</kbd> again
3. **Toolkit** > **Sleep Chart** from the main menu that is on the top (a.k.a menu bar)

# Timeline tab
Once you launch Sleep Chart, you will see an empty timeline which would look like this:

![](/supermemo/sleep-chart/empty-timeline.png)

To make it easier to understand what the buttons are, the image above has been annotated. It will also serve as a point of reference in the future.

To log a sleep block, follow the instructions below (which were taken from the official [manual](https://help.supermemo.org/wiki/Sleep_Chart#Sleep_timeline)):
> To log a block of sleep, click the beginning of the block (sleep start) and then click the end of the block (sleep end). You can also start from clicking the end of sleep first. Sleep blocks above 22 hours are disallowed. Sleep blocks cannot overlap with repetitions timeline (you cannot learn with SuperMemo and be asleep at the same time).
{.is-warning}

## An example of a filled timeline:
![](/supermemo/sleep-chart/filled-timeline.png)

Have a look at the example above. We can see <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> and <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red</span> blocks. We can also see blocks that fade from <span style="padding: 3px; color: rgb(255, 255, 255); background-color: rgb(0, 0, 0);">black</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> and blocks that fade from <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: magenta;">pink</span>.

Great. But what do they mean?
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> represents sleep blocks.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red</span> represents learning blocks. When you use SuperMemo, Sleep Chart keeps track of the time you spend working and generates these blocks. These are collection-specific blocks (in other words, each collection will show these blocks differently, depending on how much you work with each of these collections).
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: magenta;">pink</span> represents interrupted sleep (e.g., by your alarm clock). You can achieve this by pressing <kbd>Ctrl</kbd>+<kbd>A</kbd> on a sleep block. You can also achieve the same thing by right-clicking on a sleep block and selecting "**Forced awakening**".
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: rgb(0, 0, 0);">black</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> represents delayed sleep (e.g., you fell asleep whilst watching TV). You can achieve this by pressing <kbd>Ctrl</kbd>+<kbd>D</kbd> on a sleep block. You can also achieve the same thing by right-clicking on a sleep block and selecting "**Delayed retirement**".

## Annotated timeline explained

From the [annotated screenshot above](/supermemo/sleep-chart/empty-timeline.png), we can see that the timeline has a bunch of buttons. Let's take a look at each one individually. The only buttons that don't need to be explained are:
- **Tabs**: these contain different analytical graphs which we will have a look at later.
- **Menu bar**: you can read about the different options on [here](https://help.supermemo.org/wiki/Sleep_Chart#SleepChart_menu).
- **Send to SuperMemo R&D**
- **Go to a specific day on the timeline**
- **Save current timeline file**
- **Open a new timeline file**

Now that it's out of the way, we can finally dive in.

## Consolidate
The "Consolidate" [button](/supermemo/sleep-chart/empty-timeline.png) unifies sleep blocks that have a small empty gap in between. Let's say you have a small 10-minute gap between two sleep blocks, pressing this button gets rid of this gap:

![](/supermemo/sleep-chart/consolidate.png)

Why might you have a small 10-minute gap between sleep blocks? Many reasons. One of which is: let's say that you woke up in the middle of the night to drink some water, and then you went back to sleep after 10 minutes. Now, your sleep has been split into two blue blocks: the first block representing the sleep time before drinking water, and the second representing the sleep time after you drank water. These two sleep blocks will be separated by a small 10-minute gap (which represents the time you took to drink water and return to bed).

## Re-compute circadian approximations
As you may have noticed, the [filled timeline](/supermemo/sleep-chart/filled-timeline.png) has some extra detail which your current timeline may not have. I'm referring to the following:
- yellow line with circles
- blue line
- red line
- aqua dots

You can enable those by pressing the "Re-compute circadian approximations" [button](/supermemo/sleep-chart/empty-timeline.png).

Once you press it, these lines and circles will appear:
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span>. This line shows you when it is best to go to bed.
- <span style="padding: 3px; color: white; background-color: red;">Red line</span>. This line shows you when it is best to wake up (naturally, without an alarm).
- <span style="padding: 3px; background-color: yellow;">Yellow line</span>. This line should fall approximately in the middle of each sleep block, and it shows the "maximum of circadian sleepiness".
- <span style="padding: 3px; border: 2px solid red; border-image: none; background-color: cyan;">Aqua dots</span>. These dots predict the dip in you alertness levels during the day. They can be used to figure out the optimal nap time.

> ### Summary:
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span> = bedtime.
> - <span style="padding: 3px; color: white; background-color: red;">Red line</span> = wake-up time.
> - <span style="padding: 3px; border: 2px solid red; border-image: none; background-color: cyan;">Aqua dots</span> = nap time.


## Show time block data
Now you may be thinking "How am I supposed to tell what time I should be going to bed if the lines are a little squiggly?"

Well, don't worry, Sleep Chart will save you from squinting at your screen trying to figure out whether the line is at 01:15 or 01:16...

How? Press the "Show time block data" [button](/supermemo/sleep-chart/empty-timeline.png). Now pick a <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> block by simply pressing on it (which will make it turn yellow)!

A menu which will replace the current [Statistics Pane](/supermemo/sleep-chart/empty-timeline.png) will appear. This menu should contain two headings, BLOCK DATA and OPTIMUM HOURS. You will notice that in the example below I have also pressed the [Re-compute circadian approximations](#re-compute-circadian-approximations) button. This is not necessary. I am doing it to demonstrate and explain the features. I have added the red and black arrows. These will be explained [later](#optimum-hours).

![](/supermemo/sleep-chart/show-time-block-data.png)

### BLOCK DATA
Under this heading, you will find various pieces of information regarding the selected block:
- **Day**: This tells you the current day number. Every time you add a new block, it will be one number higher than the previous one. The first sleep block which you recorded will be **Day=1**, the second will be **Day=2**, and so one.
- **Date**: This displays the date at which the sleep block has started. So, the example above is showing that this sleep block has started on the Friday, 2nd of July, 2021.
- **Block**: This shows the start and finish time of the block. This particular sleep block has started at 00:51 (bedtime) and ended at 07:57 (wake-up time).
- **Length**: This displays the length of the sleep block. So, the [one above](/supermemo/sleep-chart/show-time-block-data.png) has lasted for 7 hours, and 6 minutes.

### OPTIMUM HOURS
This is the one that will provide an answer to the question we posed before: "How am I supposed to tell what time I should be going to bed if the lines are a little squiggly?"
- **Today**: This tells you when you should go to bed and when you should wake up. In this example, this Sleep Chart function has given us the exact position of the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span>, which is 01:18. This function has also given us the exact position of the <span style="padding: 3px; color: white; background-color: red;">red line</span>, which is 08:07. As we explained in the [section](#show-time-block-data) above, <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> means bedtime, and <span style="padding: 3px; color: white; background-color: red;">red line</span> means wake-up time.
- **Tomorrow**: This shows the exact same thing as **Today**, except it shows the optimum bedtime and wake-up time for tomorrow.
- **Sleep length**: This is the recommended sleep duration based on the hours shown above. So, between **Today** and **Tomorrow**, the difference in ideal sleep length hours is shown as "06:48 -> 06:52." Subtracting the hours supplied in **Today** yields the optimum amount of sleep hours for today: 08:07-01:18=06:48. The same is true for the ideal number of sleep hours for the tomorrow: 07:47-00:56=06:51.

