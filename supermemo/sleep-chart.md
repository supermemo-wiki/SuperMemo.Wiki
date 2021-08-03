---
title: SuperMemo Sleep Chart
description: A simplified version of the official SuperMemo Sleep Chart manual.
published: true
date: 2021-08-03T18:37:30.976Z
tags: 
editor: markdown
dateCreated: 2021-07-01T20:09:30.684Z
---

> Please keep in mind that this page is a work-in-progress. When this banner vanishes, you'll know this article is done. Follow the steps indicated [here](https://www.supermemo.wiki/en/home#editing-this-wiki) if you would like to contribute.
>
> As always, your feedback is greatly valued. Let us know what you liked most/least about this guide!
>
> Thank you!
{.is-warning}

# Introduction
This guide is a simplified version of the [official manual](https://help.supermemo.org/wiki/Sleep_Chart).

Whenever feasible, I've added brief summaries throughout this guide. They will look something like this:
> ### Summary
> - This is a summary!

Finally, if you've been following this page's development, then you can see the changelog [here](#changelog)!

# What is it? Who is it for?
Sleep Chart is a feature that comes with the SuperMemo software. As the name indicates, it is used to record your sleep.

Sleep Chart is for anyone who has ever searched up online or thought about something along the lines of:
- When is the best time for studying?
- When should I go to bed?
- When should I wake up?
- Should I take a nap? If so, when?

To answer these questions as accurately as possible, the user must have sufficient data.

Furthermore, please take time to read the following disclaimer from the official manual, written by [Dr. Piotr Wozniak](https://www.supermemo.wiki/en/supermemo/piotr-wozniak):
> **Important!** Your natural instinct should always take precedence over mathematical models. Moreover, best results in sleep optimization are accomplished in free-running sleep. If you use an alarm clock, or force yourself awake through the night, or take sleeping pills, the models may not adequately account for the chaotic change that is occurring in your sleep control systems.
{.is-info}

# How to access it
Accessing Sleep Chart can be done via three methods:
1. Press the <kbd>F12</kbd> button on your keyboard.
2. Press <kbd>Ctrl</kbd>+<kbd>Enter</kbd> which will bring up SuperMemo Commander. Then begin to type in the word "sleep chart" until you see it appear on the menu. Once it appears, press <kbd>Enter</kbd>.
3. **Toolkit** > **Sleep Chart** from the main menu that is on the top (a.k.a menu bar).

# Timeline tab
Once you launch Sleep Chart, you will see an empty timeline which would look like this:

![](/supermemo/sleep-chart/empty-timeline.png)

To make it easier to understand what the buttons are, the image above has been annotated. It will also serve as a point of reference in the future.

To log a sleep block, follow the instructions below (which were taken from the [official manual](https://help.supermemo.org/wiki/Sleep_Chart#Sleep_timeline)):
> To log a block of sleep, click the beginning of the block (sleep start) and then click the end of the block (sleep end). You can also start from clicking the end of sleep first. Sleep blocks above 22 hours are disallowed. Sleep blocks cannot overlap with repetitions timeline (you cannot learn with SuperMemo and be asleep at the same time).
{.is-warning}

From the [annotated screenshot above](/supermemo/sleep-chart/empty-timeline.png), we can see that the timeline has a bunch of buttons. Let's take a look at each one individually. The only buttons that don't need to be explained are:
- **Tabs**: These contain different analytical graphs which we will have a look at later.
- **Menu bar**: You can read about the different options on [here](https://help.supermemo.org/wiki/Sleep_Chart#SleepChart_menu).
- **Send to SuperMemo R&D**
- **Go to a specific day on the timeline**
- **Save current timeline file**
- **Open a new timeline file**
- I've added a green box to the bottom-left corner of the annotated screenshot. The cursor's position is displayed in this box. You'll notice that the time and dates change as you move your pointer around the timeline. Give it a go! We can also see that there is an extra value at the bottom-left corner of the [filled timeline below](/supermemo/sleep-chart/filled-timeline.png): `(length=04:10)`. This displays the length of the sleep block where the pointer is now located.

## Filled timeline example
![](/supermemo/sleep-chart/filled-timeline.png)

Before we explain what each of the buttons do, let's have a look at the [filled example above](/supermemo/sleep-chart/filled-timeline.png) (taken from the official manual).

We can see the following:
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue blocks</span>.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">Red blocks</span>.
- Blocks that fade from <span style="padding: 3px; color: rgb(255, 255, 255); background-color: rgb(0, 0, 0);">black</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span>.
- Blocks that fade from <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: magenta;">pink</span>.

Great! But what do they mean?!
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue blocks</span> represent sleep episodes.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">Red blocks</span> represents learning time. When you use SuperMemo, Sleep Chart keeps track of the time you spend working and generates these blocks. These are collection-specific blocks (in other words, each collection will show these blocks differently, depending on how much you work with each of these collections).
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: magenta;">pink</span> blocks represent interrupted sleep (e.g., by your alarm clock). You can achieve this by pressing <kbd>Ctrl</kbd>+<kbd>A</kbd> on a sleep block. You can also achieve the same thing by right-clicking on a sleep block and selecting "**Forced awakening**".
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: rgb(0, 0, 0);">Black</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> blocks represent delayed sleep (things such "falling asleep whilst watching TV" and "not being able to sleep straight after going to be" are considered to be delayed sleep). You can achieve this by pressing <kbd>Ctrl</kbd>+<kbd>D</kbd> on a sleep block. You can also achieve the same thing by right-clicking on a sleep block and selecting "**Delayed retirement**".

> ### Summary:
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue blocks</span> = sleep.
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">Red blocks</span> = time spent studying with SuperMemo.
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: magenta;">pink</span> blocks = interrupted sleep. Use <kbd>Ctrl</kbd>+<kbd>A</kbd> to mark a sleep block as interrupted.
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: rgb(0, 0, 0);">Black</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> blocks = delayed sleep. Use <kbd>Ctrl</kbd>+<kbd>D</kbd> to mark a sleep block as delayed.

## Consolidate
The "Consolidate" [button](/supermemo/sleep-chart/empty-timeline.png) unifies sleep blocks that have a small empty gap in between. Let's say you have a small 10-minute gap between two sleep blocks, pressing this button gets rid of this gap:

![](/supermemo/sleep-chart/consolidate.png)

Why might you have a small 10-minute gap between sleep blocks? Many reasons. Let's say that you woke up in the middle of the night to drink some water, and then you went back to sleep after 10 minutes. Now, your sleep has been split into two blue blocks: the first block representing the sleep time before drinking water, and the second representing the sleep time after you drank water. These two sleep blocks will be separated by a small 10-minute gap (which represents the time you took to drink water and return to bed).

## Re-compute circadian approximations
As you may have noticed, the [filled timeline](/supermemo/sleep-chart/filled-timeline.png) has some extra detail which your current timeline may not have. I'm referring to the following:
- Yellow line with circles
- Blue line
- Red line
- Aqua dots

You can enable those by pressing the "Re-compute circadian approximations" [button](/supermemo/sleep-chart/empty-timeline.png).

Once you press it, these lines and circles will appear. Now, let's have a look at what they mean:
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span>: This line shows you when it is best to go to bed.
- <span style="padding: 3px; color: white; background-color: red;">Red line</span>. This line shows you when it is best to wake up (naturally, without an alarm).
- <span style="padding: 3px; background-color: yellow;">Yellow line</span>: This line should fall approximately in the middle of each sleep block, and it shows the "maximum of circadian sleepiness".
- <span style="padding: 3px; border: 2px solid red; border-image: none; background-color: cyan;">Aqua dots</span>: These dots predict the dip in you alertness levels during the day. They can be used to figure out the optimal nap time.

> ### Summary:
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span> = predicted bedtime.
> - <span style="padding: 3px; color: white; background-color: red;">Red line</span> = predicted wake-up time.
> - <span style="padding: 3px; border: 2px solid red; border-image: none; background-color: cyan;">Aqua dots</span> = predicted nap time.

## Show time block data
Now you may be thinking "How am I supposed to tell what time I should be going to bed if the lines are a little squiggly?"

Well, don't worry, Sleep Chart will save you from squinting at your screen trying to figure out whether the line is at 01:15 or 01:16...

How? Press the "Show time block data" [button](/supermemo/sleep-chart/empty-timeline.png). Now pick a <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> block by simply pressing on it (which will make it turn yellow)!

A new menu on the right side of the window will appear (replacing the current [Statistics Pane](#statistics-pane)). This menu should contain two headings, [BLOCK DATA](#block-data) and [OPTIMUM HOURS](#optimum-hours).

You will notice that in the example below I have pressed the [Re-compute circadian approximations](#re-compute-circadian-approximations) button. This is not required. I am doing it to demonstrate and explain the features. I have also added the red and black arrows. These will be explained [later](#optimum-hours).

![](/supermemo/sleep-chart/show-time-block-data.png)

### BLOCK DATA
Under this heading, you will find various pieces of information regarding the selected block:
- **Day**: This tells you the day number ever since you started logging your sleep. The first sleep block which you recorded will be **Day=1**.
- **Date**: This displays the date at which the sleep block has started. So, the [example above](/supermemo/sleep-chart/show-time-block-data.png) is showing that this sleep block has started on the Friday, 2nd of July, 2021.
- **Block**: This shows the start and finish time of the block. This particular sleep block has started at 00:51 (bedtime) and ended at 07:57 (wake-up time).
- **Length**: This displays the length of the sleep block. So, the [one above](/supermemo/sleep-chart/show-time-block-data.png) has lasted for 7 hours, and 6 minutes.

### OPTIMUM HOURS
This is the one that will provide an answer to the question we posed before: "How am I supposed to tell what time I should be going to bed if the lines are a little squiggly?"
- **Today**: This tells you when you should go to bed and when you should wake up. In this example, this Sleep Chart function has given us the exact position of the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span>, which is 01:18. This function has also given us the exact position of the <span style="padding: 3px; color: white; background-color: red;">red line</span>, which is 08:07. As we explained in the [section above](#show-time-block-data): <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> means bedtime and <span style="padding: 3px; color: white; background-color: red;">red line</span> means wake-up time. I have used the red arrows in the [screenshot above](/supermemo/sleep-chart/show-time-block-data.png) to help you understand this further.
- **Tomorrow**: This shows the exact same thing as **Today**, except it shows the optimum bedtime and wake-up time for tomorrow. I have used the black arrows in the [screenshot above](/supermemo/sleep-chart/show-time-block-data.png) to help you understand this further.
- **Sleep length**: This is the recommended sleep duration based on the hours shown above. So, the change in ideal sleep length between **Today** and **Tomorrow** is shown as `06:48 -> 06:52`. You can skip the next sentence as it's there for context. Subtracting the hours supplied in **Today** yields the optimum amount of sleep hours for today: `08:07 - 01:18 = 06:48`. The same is true for **Tomorrow**: `07:47 - 00:56 = 06:51`.

### Statistics Pane
There is a pane on the right side of the window, as seen in the [annotated screenshot](/supermemo/sleep-chart/empty-timeline.png). Let's call it the Statistics Pane (though it is worth mentioning that this is not the official name).

This pane displays various statistics about the individual days. You can cycle through these options by pressing <kbd>Ctrl</kbd>+<kbd>Right</kbd> and <kbd>Ctrl</kbd>+<kbd>Left</kbd>. The statistics are fairly self-explanatory, and hence we will not go through them in detail for now.

You can also click on Options from the [Menu bar](/supermemo/sleep-chart/empty-timeline.png), then choose Statistics.

# Circadian tab
This tab gives you a greater insight into your sleep time. According to Dr. Piotr Wozniak: "you will need a couple of months of data before this graph becomes meaningful."

There are two graph views in this tab: [Hours from arising](#hours-from-arising) and [Clock time](#clock-time).

## Hours from arising
This is the default view. The annotated screenshot below shows you what this view is like. It also introduces you to the new buttons:

![](/supermemo/sleep-chart/circadian-hrs-arising.png)

First of all, let's see what the above is showing, and then we will have a look at some [sample data interpretation](#sample-data-interpretation-hours-from-arising):
- Left vertical axis shows the sleep length.
- Right vertical axis shows the "percentage of sleep episodes initiated at any given time".
- Horizontal axis could be interpreted in two ways (depending on whether or not you click the "Switch between absolute hours and relative hours" [button](/supermemo/sleep-chart/circadian-hrs-arising.png)). The example above is showing hours from arising. So, the number 0 on the horizontal axis is referring to the waking hour. If you press the previously mentioned button, you will notice three things: first, the graph will change dramatically, and second, the horizontal axis will now read "Clock time" (24-hour clock). Finally, you will notice that the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">green line</span> has disappeared.
- The little <span style="padding: 3px; border: 1px solid rgb(149, 172, 195); border-image: none; color: white; background-color: rgb(165, 207, 248);">light blue dots</span> represent the sleep blocks we talked about in the [section above](#an-example-of-a-filled-timeline). So, each light blue dot represents a sleep episode.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span> represents the bedtime frequency. The higher is the peak, the more frequent is the bedtime. Use the right vertical axis to determine the value of this line.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">Red line</span> represents the average sleep length. Use the left vertical axis to determine the value of this line.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">Green line</span> splits the graph into two sections, phase advanced (right) and phase delays (left). The way this line works is by following <span style="padding: 3px; border: 1px solid rgb(149, 172, 195); border-image: none; color: white; background-color: rgb(165, 207, 248);">light blue dots</span> where the waking time (horizontal axis) and the sleep time (left vertical axis) add up to 24 hours.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">Green line</span> crossing the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span> shows the "optimum balanced sleep cycle of 24 hours".

> ### Summary:
> - Left vertical axis = sleep length.
> - Right vertical axis = percentage of sleep episodes initiated at any given time.
> - Horizontal axis = relative/absolute hours.
> - <span style="padding: 3px; border: 1px solid rgb(149, 172, 195); border-image: none; color: white; background-color: rgb(165, 207, 248);">Light blue dots</span> = sleep blocks we talked about in the [section above](#an-example-of-a-filled-timeline).
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span> = bedtime frequency. Use the right vertical axis to determine the value of this line.
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">Red line</span> = average sleep length. Use the left vertical axis to determine the value of this line.
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">Green line</span> = separates the graph into two sections: phase advanced (right) and phase delays (left).
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">Green line</span> crossing the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span> = "optimum balanced sleep cycle of 24 hours".

## Sample data interpretation (Hours from arising)
From the [screenshot above](/supermemo/sleep-chart/circadian-hrs-arising.png), we can infer the following:
- Most frequent bedtime occurs after 17 hours from arising (because that's where the SECOND peak (from the left) of the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> occurs). In fact, 19.9% of the sleep episodes have occurred after 17 hours from arising (we used the right vertical axis to determine this value).
- Most frequent nap time occurs after 7 hours from arising (because that's where the FIRST peak (from the left) of the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> occurs).
- On average, the naps last for about 1 hour and 30 minutes (because the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span> is around this area. See the black dashed line which I added to the [screenshot above](/supermemo/sleep-chart/circadian-hrs-arising.png)).
- In this example, 17 hours from arising, the user is expected to sleep for 7 hours (because that's where the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">green line</span> crosses the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span>. See the two black arrows which I added to the [screenshot above](/supermemo/sleep-chart/circadian-hrs-arising.png)). Also notice that 17 hours plus 7 hours is equal to 24 hours!

## Clock time
Now, you might be thinking "The [Circadian tab](#circadian-tab) is awesome, but figuring out the most frequent bedtime on a 24-hour clock using the 'hours from arising' method is a little challenging."

Fear not, Sleep Chart has got you covered! Click the "Switch between absolute and relative hours" [button](/supermemo/sleep-chart/circadian-hrs-arising.png) to get the Clock time graph. Again, we will have a look at some [sample data interpretation](#sample-data-interpretation-clock-time) after discussing the screenshot below:

![](/supermemo/sleep-chart/circadian-hrs-clock.png)

As we discussed earlier, the horizontal axis can be interpreted in two ways: absolute and relative hours. And as we saw earlier, pressing the "Switch between absolute and relative hours" [button](/supermemo/sleep-chart/circadian-hrs-arising.png) changes the graph dramatically by:
- Shifting the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> and the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span>.
- Switching horizontal axis from "Hours from arising" to "Clock time".
- Removing the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">green line</span>.

Other than those changes outlined above, everything else is still the same: the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> still means "bedtime frequency", and the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span> still means "average sleep length".

## Sample data interpretation (Clock time)
From the [screenshot above](/supermemo/sleep-chart/circadian-hrs-clock.png), we can infer the following:
- Most frequent bedtime occurs at 01:00 (because that's where the FIRST peak (from the left) of the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> occurs). In fact, 36.4% of the sleep episodes have occurred at this time (we used the right vertical axis to determine this value).
- If the user sleeps at this most frequent bedtime, they would get (on average) 7 hours of sleep (because the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span> is around this area).
- Most frequent nap time occurs at 16:00 (because that's where the SECOND peak (from the left) of the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span> occurs).
- Once again, on average, the naps last for about 1 hour and 30 minutes (because the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span> is around this area).

## Learning Circadian Cycle
We've discussed sleep exhaustively. Let's now turn our attention to something equally vital: learning.

As you may recall, there were some <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red blocks</span> present in the [timeline tab](#timeline-tab). We learned that these blocks represent time spent studying with SuperMemo.

These blocks are also represented by a graph to help you spot trends and, hence, determine the best time to learn. Simply click the "Switch between sleep data and repetition data" [button](/supermemo/sleep-chart/circadian-hrs-arising.png) to get this graph!

The interpretation of the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span>, <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span>, and the 3 axes is exactly the same as before. Therefore, we will not go through them again now.

In case you still require some extra guidance, I have annotated the graph below:

![](/supermemo/sleep-chart/learning-circadian-cycle.png)

.
.
.
.
.
.
.
.
.
.
.
.
# Changelog
## 3rd of August, 2021
- Updated the meaning of the term "[delayed retirement](#filled-timeline-example)"
- Added some more information to [Learning Circadian Cycle](#learning-circadian-cycle) section
- Added picture to [Learning Circadian Cycle](#learning-circadian-cycle) section
- Updated the summary for [Re-compute circadian approximations](#re-compute-circadian-approximations) section

## 1st of August, 2021
- Updated the picture used in [Clock time](#clock-time) section
- Added [Learning Circadian Cycle](#learning-circadian-cycle) section
- Other edits