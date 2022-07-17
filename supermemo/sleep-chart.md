---
title: SuperMemo Sleep Chart
description: A simplified version of the official SuperMemo Sleep Chart manual.
published: true
date: 2022-07-17T13:05:30.137Z
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
Accessing Sleep Chart can be done via three ways:
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

## Sample timeline
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
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: rgb(0, 0, 0);">Black</span> to <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue</span> blocks represent delayed sleep (things such "falling asleep whilst watching TV" and "you did not go to sleep because you were working" are considered to be delayed sleep). You can achieve this by pressing <kbd>Ctrl</kbd>+<kbd>D</kbd> on a sleep block. You can also achieve the same thing by right-clicking on a sleep block and selecting "**Delayed retirement**".

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
- The little <span style="padding: 3px; border: 1px solid rgb(149, 172, 195); border-image: none; color: white; background-color: rgb(165, 207, 248);">light blue dots</span> represent the sleep blocks we talked about in the [section above](#sample-timeline). So, each light blue dot represents a sleep episode.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span> represents the bedtime frequency. The higher is the peak, the more frequent is the bedtime. Use the right vertical axis to determine the value of this line.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">Red line</span> represents the average sleep length. Use the left vertical axis to determine the value of this line.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">Green line</span> splits the graph into two sections, phase advanced (right) and phase delays (left). The way this line works is by following <span style="padding: 3px; border: 1px solid rgb(149, 172, 195); border-image: none; color: white; background-color: rgb(165, 207, 248);">light blue dots</span> where the waking time (horizontal axis) and the sleep time (left vertical axis) add up to 24 hours.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: green;">Green line</span> crossing the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span> shows the "optimum balanced sleep cycle of 24 hours".

> ### Summary:
> - Left vertical axis = sleep length.
> - Right vertical axis = percentage of sleep episodes initiated at any given time.
> - Horizontal axis = relative/absolute hours.
> - <span style="padding: 3px; border: 1px solid rgb(149, 172, 195); border-image: none; color: white; background-color: rgb(165, 207, 248);">Light blue dots</span> = sleep blocks we talked about in the [section above](#sample-timeline).
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


# Phase shift tab
People with [Advanced Sleep Phase Disorder (ASPD)](https://en.wikipedia.org/wiki/Advanced_sleep_phase_disorder) and [Delayed Sleep Phase Disorder (DSPD)](https://en.wikipedia.org/wiki/Delayed_sleep_phase_disorder) might benefit from this tab. However, you can still use it to work out the "expected bedtime given a specific natural waking time."

![](/supermemo/sleep-chart/phase-shift-tab.png)

As usual, let's dissect the graph above before having a look at some [sample data interpretation](#sample-data-interpretation-phase-shift-tab):
- Left vertical axis shows the bedtime hours. And, just like in the horizontal axis in the [Circadian tab](#circadian-tab), this axis has two options (which can be modified using the "Switch between absolute hours and relative hours" [button](/supermemo/sleep-chart/phase-shift-tab.png)): hours from arising and clock time.
- Horizontal axis shows the natural waking hour (24-hour clock).
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue line</span> shows "the bedtime for days with a given waking hour." Use the left vertical axis to determine the value of this line.
- <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">Red line</span> shows the "next day's waking hours." Use the horizontal axis to determine the value of this line.
- <span style="padding: 3px; background-color: fuchsia;">Fuchsia line</span> and <span style="padding: 3px; background-color: silver;">gray line</span> show the siesta/nap period.

## Sample data interpretation (Phase shift tab)
Here's a free tip from me to you: the simplest way to interpret this graph is to begin with the horizontal axis.

> Please keep in mind that these are only estimates, *not* recommendations. If the value provided by Sleep Chart appears to be absurd, then apply your judgement and trust your natural instincts (i.e., you must go to sleep if you feel tired). Furthermore, as it has been previously indicated, the graphs are only accurate if you free-run your sleep.
{.is-warning}

Let's have a look at the [annotated screenshot above](/supermemo/sleep-chart/phase-shift-tab.png). If the user wakes up at 07:00 (horizontal axis), then:
- Using the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">blue line</span>, we can see that their bedtime will occur at around 00:30 (vertical axis).
- Using the <span style="padding: 3px; color: rgb(255, 255, 255); background-color: red;">red line</span>, we can see that the user will wake up at around 07:10 the next day.
- Using the <span style="padding: 3px; background-color: fuchsia;">fuchsia line</span> and <span style="padding: 3px; background-color: silver;">gray line</span>, we can see that the expected nap period for that given hour is between 15:00 (<span style="padding: 3px; background-color: silver;">gray line</span>) and 16:30 (<span style="padding: 3px; background-color: fuchsia;">fuchsia line</span>).

# Alertness tab
Before we get started, I should tell you that things are going to become wild. I personally struggled to grasp this topic in such a short amount of time, and as a result, I fear that I may provide you with incorrect information. However, I intend to return to this article (when I have more free time) to double-check that everything is correct. So, I advise you that you refer to [official manual](https://help.supermemo.org/wiki/Sleep_Chart) just to be safe!

So, without further ado, let's get down to business.

To fully comprehend this tab, you must first understand two key sleep principles. These are the components of sleep:
1. **Homeostatic component**: the more we stay awake, the sleepier we get.
2. **Circadian component**: sleep is a 24-hour cycle, which peaks and troughs. The word "circadian" comes from the Latin "circa diem", which means "around a day."

You got all that? Cool.

Simply said, "alertness" in SuperMemo refers to "how alert you are when studying." This is calculated using the average grade in learning with SuperMemo, according to Dr. Wozniak. So, if you get better grades in the morning and worse grades in the evening, it's likely that you're more alert in the morning.

For the keen-eyed among you, you may have noticed that there are TWO Alertness tabs: **Alertness (H)** and **Alertness \(C\)**. You've probably figured it out by now.

**Alertness (H)**: this is the homeostatic alertness, which is a measurement of alertness *since that last sleep episode*.

**Alertness \(C\)**: this is the circadian alertness, which is a measurement of alertness *with respect to the circadian time (i.e., "time measured since the optimum natural waking hour")*. This is a little trickier to understand, I know.

I have [asked for a better explanation](https://supermemopedia.com/wiki/Sleep_Chart:_Alertness_(H)_vs._Alertness_(C)) of the differences between the two, and here is the response that I got:
> Alertness can be studied in reference to homeostatic (H) and circadian (C) variables, however, those variables cannot be easily disentangled. High alertness is the effect of maximum circadian alertness and minimum homeostatic fatigue. That state can be safely marked as the state that maximizes alertness for both variables. This state should characterize early morning in a healthy sleep cycle. However, low alertness may be caused by changes in any of the alertness variables. When both H and C variables show alertness minima, natural sleep occurs.
> 
> Circadian alertness shows how alertness changes during a waking day. It is plotted against the waking time.
> 
> Homeostatic alertness cannot be separated from circadian variables except for a short period after waking when it declines exponentially.
> 
> This is why homeostatic alertness plotted against waking day that is not interrupted by sleep is the closes approximation of homeostatic drop in mental efficiency.
> 
> In non-nappers the graphs may turn out similar as the homeostatic curve may span beyond the circadian dip in alertness followed by seeming "recovery".
> 
> https://supermemo.guru/wiki/Sleep_and_learning#Alertness_multiplier

I also got a better definition of the terms "natural [waking hour](https://supermemopedia.com/wiki/Waking_time)" and "last [sleep episode](https://supermemopedia.com/wiki/Sleep_episode)":
> **Waking time** is the time of waking up. If you wake up and look at the clock, and it is 9:11, you can say this is your waking time. This may differ from expected natural waking time that depends on the circadian cycle.
> 
> **Sleep episode** is a single block of sleep marked by waking time before and after. A sleep episode may be shorter than night sleep. For example, if you wake up at 4:20 am to visit the toilet, your sleep episodes might be 23:23-4:20 and 4:26-7:46.

# Napping tab
As the name suggests, this tab is for the napping graphs. According to Dr. Wozniak, if your night sleep is shortened, you tend to compensate with naps.

Have a look at the [screenshot below](/supermemo/sleep-chart/napping.png). I have annotated and explained it.

Note: The size of the blue dots reflects how much information is available. As a result, the larger the dot, the more data is collected, and thus the plot is more accurate.

![](/supermemo/sleep-chart/napping.png)

# Learning tab
In this tab, you can have a look at the correlation between your sleep and the number of learning hours.

![]()

> ### Summary
> - Vertical axis = sleep obtained in the first 11 hours from bedtime (?)
> - Horizontal axis = 

# Consolidation tab
.

# Two-component sleep model
SuperMemo predicts the homeostatic and circadian status of overall sleep propensity (i.e., how sleepy you feel) based on the user's sleep data. This is, without a doubt, my favourite Sleep Chart feature. It's something I use on a daily basis.

To access this graph (faster):
1. Hold <kbd>Shift</kbd> on your keyboard and press on a day row in the [Timeline tab](#timeline-tab)

Another way to access this graph:
1. Right click on a sleep block in the [Timeline tab](#timeline-tab)
2. Select "Sleep propensity" (you can also use <kbd>Ctrl</kbd>+<kbd>P</kbd>)

You will notice that there are many lines on this graph. I, personally, only use 2 of them: the <span style="padding: 3px; color: white; background-color: red;">red line</span> and the <span style="padding: 3px; background-color: aqua;">aqua line</span>. These two are the ones which provide the most useful/interesting information.

![](/supermemo/sleep-chart/two-component.png)

> ### Summary
> - <span style="padding: 3px; color: rgb(255, 255, 255); background-color: blue;">Blue blocks</span> = actual sleep episodes (see [Sample timeline](#sample-timeline) for more information about these blocks).
> - <span style="padding: 3px; background-color: aqua;">Aqua line</span> = 24-hour circadian sleep propensity. The peaks mean that you are more sleepy, and thus, a nap is good idea. If you remember, the <span style="padding: 3px; border: 2px solid red; border-image: none; background-color: cyan;">aqua dots</span> that we talked about in the [Re-compute circadian approximations](#re-compute-circadian-approximations) section above predicted the nap time. Now, the peak of if this <span style="padding: 3px; background-color: aqua;">aqua line</span> represents the <span style="padding: 3px; border: 2px solid red; border-image: none; background-color: cyan;">aqua dots</span>.
>   - ***In short: peak of <span style="padding: 3px; background-color: aqua;">aqua line</span> = <span style="padding: 3px; border: 2px solid red; border-image: none; background-color: cyan;">aqua dot</span> on [Timeline tab](#timeline-tab) = predicted optimum nap time.***
> - <span style="padding: 3px; color: white; background-color: green;">Green line</span> = an inverse of the homeostatic sleep propensity
> - <span style="padding: 3px; background-color: yellow;">Yellow vertical lines</span> = circadian middle-of-the-night peak. I believe that this represents the <span style="padding: 3px; background-color: yellow;">Yellow lines</span> in [Timeline tab](#timeline-tab) (see [Re-compute circadian approximations](#re-compute-circadian-approximations) section for more information).
> - <span style="padding: 3px; color: white; background-color: red;">Red line</span> = resultant alertness. The higher the peak, the more alert you are *predicted* to be.
> - <span style="padding: 3px; background-color: fuchsia;">Vertical fuchsia line</span> = marks the 24th hour (i.e., the end of the day/start of a new day)


# Changelog
## 29th of April, 2022
- Updated [Alertness tab](#alertness-tab) section (it's still a work-in-progress).
- Added [Two-component sleep model tab](#two-component-sleep-model).
- Added [Learning tab](#learning-tab) (it's still a work-in-progress).
- Added [Consolidation tab](#consolidation-tab) (it's still a work-in-progress).
- Other edits

## 14th of February, 2022
- I have not abandoned the article, I promise!
- Added the [Alertness tab](#alertness-tab) section (it's still a work-in-progress).
- Added the [Napping tab](#napping-tab) section

## 20th of August, 2021
- Added [Phase shift tab](#phase-shift-tab) section and added a picture
- Updated the meaning of the term "[delayed retirement](#sample-timeline)" (again...)

## 3rd of August, 2021
- Updated the meaning of the term "[delayed retirement](#sample-timeline)"
- Added some more information to [Learning Circadian Cycle](#learning-circadian-cycle) section
- Added picture to [Learning Circadian Cycle](#learning-circadian-cycle) section
- Updated the summary for [Re-compute circadian approximations](#re-compute-circadian-approximations) section

## 1st of August, 2021
- Updated the picture used in [Clock time](#clock-time) section
- Added [Learning Circadian Cycle](#learning-circadian-cycle) section
- Other edits