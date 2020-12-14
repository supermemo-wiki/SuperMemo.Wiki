---
title: Introduction to SuperMemo
description: Essential concepts to understand SuperMemo.
published: true
date: 2020-12-14T10:47:24.459Z
tags: 
editor: markdown
dateCreated: 2020-12-05T18:34:19.777Z
---

# What is SuperMemo?

[**SuperMemo**](https://super-memo.com/supermemo18.html){target="_blank"} is a program that **makes learning easy and fun**.

SuperMemo is built on two novel learning techniques named [Spaced Repetition](/learning/spaced-repetition) and [Incremental Reading](/learning/incremental-reading) pioneered by Dr. [Piotr Wozniak](/supermemo/piotr-wozniak)[^1], the inventor of SuperMemo. They enable anyone to form long-lasting memories, and to gain new knowledge more efficiently compared with traditional techniques.

While the success of SuperMemo is often attributed to its cutting-edge  algorithms and techniques, Dr. Piotr Wozniak and many <abbr title="Users who have been using SuperMemo for a duration ranging from a few years, up to several decades.">long-time users</abbr> of SuperMemo[^2] emphasize the central importance of [Pleasure of Learning](/learning/pleasure-of-learning) in all forms of learning activities.

## Why can SuperMemo change your life?

Here are a few reasons why SuperMemo might **improve your life**:

### Tabs{.tabset}
#### I am Human

1. **You can learn to love learning (again):**
    - Learning is the best way to improve your life,
    - SuperMemo is built to make learning pleasurable,
    - As you progressively learn to love learning, your life will gradually improve!
2. **You can meet amazing people:**
    - [Our community](https://discord.gg/vUQhqCT) is oustandingly supportive and caring,
    - You will have discussions on topics that you cannot have elsewhere,
    - These discussions will spark new ideas and projects.

#### I am a Student (TODO)

🚧 Work in progress.

#### I am Salaried[^3] (TODO)

🚧 Work in progress.

#### I am a Policy Maker

1. **You can learn to better handle complexity**
    - Understanding politics and societies demands a lot of knowledge,
    - SuperMemo is built to handle large volume of information,
    - You will become more informed, and better equipped to make good decisions.
2. **You can spread the word**
    - Once you rediscover the pleasure of learning, you will be able to promote policies that encourage it,
    - People will become more educated, and more happy.

## Spaced Repetition

> Main article: [Spaced Repetition](/learning/spaced-repetition)
{.is-info}

🚧 Work in progress.

## Incremental Reading

**Incremental Reading (IR)** is a technique for organizing learning in a way that privileges *variety of studying material*. By contrast, traditional reading involves a linear process of reading a single topic extended periods of time.

In the context of this wiki, **material** designates any sort of media through which learning can be achieved. Some example of material include: books, web articles, videos, podcasts, etc.

### Comparison Matrix

This table **compares the principles** of incremental reading (parallel) and traditional reading (linear), based on their *average* implementation and usage. This is not representative of all the variations in which both of these methods can be executed.

<table>
  <tbody>
    <tr>
      <td width="200">
        <p>
          <strong> </strong>
        </p>
      </td>
      <td width="200">
        <p>
          <strong>Incremental Reading</strong>
        </p>
      </td>
      <td width="200">
        <p>
          <strong>Traditional Reading</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <strong>Mindset</strong>
        </p>
      </td>
      <td>
        <p>Read material until concentration or pleasure dwindles.</p>
      </td>
      <td>
        <p>Read material for as long as possible.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <strong>Variety of material</strong>
        </p>
      </td>
      <td>
        <p>Many (up to hundreds).</p>
      </td>
      <td>
        <p>Few (less than a dozen).</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <strong>Avg. Duration<sup>*</sup></strong>
        </p>
      </td>
      <td>
        <p>Seconds to minutes for each material.</p>
      </td>
      <td>
        <p>Hours for each material.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <strong>Min/Max Duration</strong>
        </p>
      </td>
      <td>
        <p>Seconds to hours for each material.</p>
      </td>
      <td>
        <p>Minutes to hours for each material.</p>
      </td>
    </tr>
  </tbody>
</table>

> **^*^**: In IR, most material is gradually broken down into smaller chunks, hence the low average duration.
>
> **Nothing precludes an incremental reader from deliberately reading one topic for hours** at a time. Typical motivations include:
> - studying for school,
> - personal keenship for a subject matter,
{.is-info}

### General flow of Incremental Reading (simplified)

In Incremental Reading, all the material yet to be processed is added into a [queue](/supermemo/queues). Each individual element in the queue is examined until the student decides to move to the next topic (in the queue). Typical triggers for making that decision include decreases in concentration or pleasure.

```mermaid

graph TB
    IR-step1>"Read article"]
    IR-step2("<img src='/supermemo/incremental-reading/ir-1st-rep-step-1.png'; width='250px' height='154px'/>")
    IR-step3("<img src='/supermemo/incremental-reading/ir-1st-rep-step-2.png'; width='250px' height='161px'/>")
    IR-step4>"Move to next article"]
    
    IR-step1 -- 1. Locate interesting information --> IR-step2
    IR-step2 -- 2. Extract valuable text for later --> IR-step3
    IR-step3 -- 3. Repeat until bored with current article --> IR-step1
    IR-step3 -- 4. When bored with current article --> IR-step4
    IR-step4 -- 5. Repeat until done with studying --> IR-step1

```

### Example: Evolution over a few days

This example illustrates the **evolution of a paragraph** taken from the [wiki article](https://en.wikipedia.org/wiki/Learning#Non-associative_learning) about *Learning*. The actual order of reviews and formulation of items might differ from person to person.

> The numbers assigned to each day are only meant as an illustration for the purpose of our example. Actual intervals between repetitions will typically be larger within SuperMemo.
>
> A more accurate term here would have been **stage**, but **day** was used instead for its intuititivity.
{.is-info}

#### Day 1 of Incremental Reading
```mermaid

graph LR
    IR-rep1-step1>"Do IR"]
    IR-rep1-step2("<p class='pt-0 mb-2'><b>Locate interesting information</b></p><img src='/supermemo/incremental-reading/ir-1st-rep-step-1.png'; width='250px' height='154px'/>")
    IR-rep1-step3("<p class='pt-0 mb-2'><b>Extract valuable text</b></p><img src='/supermemo/incremental-reading/ir-1st-rep-step-2.png'; width='250px' height='161px'/>")
    IR-rep1-step4>"Continue IR"]
    
    IR-rep1-step1 --> IR-rep1-step2
    IR-rep1-step2 --> IR-rep1-step3
    IR-rep1-step3 --> IR-rep1-step4

```

#### Day 2 of Incremental Reading
```mermaid

graph LR
    IR-rep2-step1>"Do IR"]
    IR-rep2-step2("<p class='pt-0 mb-2'><b>Extracted text from Day 1 comes up</b></p><img src='/supermemo/incremental-reading/ir-2nd-rep-step-1.png'; width='250px' height='93px'/>")
    IR-rep2-step3("<p class='pt-0 mb-2'><b>Create a <i>fill the blank</i> question</b></p><img src='/supermemo/incremental-reading/ir-2nd-rep-step-2.png'; width='250px' height='98px'/>")
    IR-rep2-step4>"Continue IR"]
    
    IR-rep2-step1 --> IR-rep2-step2
    IR-rep2-step2 --> IR-rep2-step3
    IR-rep2-step3 --> IR-rep2-step4
```

#### Day 3 of Incremental Reading
```mermaid

graph TB
    IR-rep3-step1["Work in progress"]
```

# Getting Started

- [First steps *Installation and Basic usage of SuperMemo.*](/supermemo/first-steps)
- [Backup Guide *Why risk losing years of work ? Set it up now, and forget about it !*](/supermemo/backup-guide)
- [Going further *Pointers for progressing to expert levels.*](/supermemo/going-further)
{.links-list}


## Video guides

- [Video guides *A series of video that will take you from Beginner to Advanced level.*](https://www.youtube.com/playlist?list=PL7RwmzKKAH8eKbDpOe5e-Omfp2Zqed6U1)
- [YouTube channel *Educative videos published by the SuperMemo.wiki community.*](https://www.youtube.com/channel/UCMdkN_8gHPn5vlYDe2ScrxQ)
{.links-list}

<div class="mt-8">
  <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/i33BTuwTgAs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

[^1]: https://supermemo.guru/wiki/History_of_spaced_repetition
[^2]: https://supermemo.guru/wiki/Declaration_of_Educational_Emancipation:_Signatories
[^3]: Word chosen on purpose. Salary does not equate income https://www.youtube.com/watch?v=eyrEykrcQi0

![SuperMemo.wiki](/supermemo-64.png){.align-abstopright}