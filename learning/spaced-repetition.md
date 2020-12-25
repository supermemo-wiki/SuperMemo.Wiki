---
title: Spaced repetition
description: 
published: true
date: 2020-12-25T07:58:43.803Z
tags: 
editor: markdown
dateCreated: 2020-12-15T21:11:31.397Z
---

**Spaced repetition (SR)** is a method for organizing your learning calendar in the most optimized way possible. It has two functions:
1. Knowledge learned this way should be remembered forever,
2. Remembering forever should use up the minimum amount of time possible.

# How does it work?

In practice SR is performed by creating **flashcards** and assigning them a [forgetting index](/supermemo/spaced-reptition#flashcards) within a computer software.

**Flashcard** is generic term for any association of knowledge. An example is the association between two words in different languages: "Hello" means "Bonjour" in French. The reciprocal association "Bonjour" -> "Hello" is another flashcard. They can be physical (paper cards) or virtual (like in SuperMemo).

![types-of-flashcard.png](/supermemo/spaced-repetition/types-of-flashcard.png =820x)

The **forgetting index** is a number that represents the likelihood (e.g. 10%) you will forget a given piece of knowledge (e.g. "Hello" -> "Bonjour") before the next date on the calendar when SR has scheduled a **review** for it. For example, if on the 1st of January you learned that "Hello" means "Bonjour" in French, you might only be able to recall that with 90% certainty until the 20th of January. Past that date, the likelihood of recalling it will keep decreasing. This is because forgetting is exponential in nature:

![forgetting-curve.png](/supermemo/spaced-repetition/forgetting-curve.png)

Forgetting is avoided by **reviewing** your knowledge. Reviewing is the process of refreshing knowledge to ensure that it is persisted in memory. For example, on the 20th of January, you might quiz yourself:
> *What is the French translation for 'Hello'?*.

If you recalled correctly, then your memory of that knowledge will be persisted for an even longer time than you previously had, for example until March 31th with a 90% recall rate.

# Comparison Matrix

<table class="content-align-top">
  <tbody>
    <tr>
      <td width="180">
        <p>
          <strong>
            <em> </em>
          </strong>
        </p>
      </td>
      <td width="250">
        <p>
          <strong>Spaced repetition</strong>
        </p>
      </td>
      <td width="250">
        <p>
          <strong>Traditional learning</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <em>Support</em>
        </p>
      </td>
      <td>
        <p>Computer software<sup><b>*</b></sup>.</p>
      </td>
      <td>
        <p>Any (usually pen &amp; paper).</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <em>Study plan</em>
        </p>
      </td>
      <td>
        <p>Automatically scheduled by the algorithm.</p>
      </td>
      <td>
        <p>Manually, either by:</p>
        <ul>
          <li>Planning in advance (e.g., for an exam),</li>
          <li>Spontaneously (re-)reading a note or a book.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <em>Scalability</em>
        </p>
      </td>
      <td>
        <p>High: the software knows everything you want to remember.</p>
      </td>
      <td>
        <p>Low: you cannot list everything you've learned and remember to review it. It is a circular problem.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <em>Time spent learning</em>
        </p>
      </td>
      <td>
        <p>Minimal: the algorithm computes the optimum interval between reviews.</p>
      </td>
      <td>
        <p>Suboptimal: reviews will be random or arbitrary (e.g., for an exam).</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <em>Chance of remembering</em>
        </p>
      </td>
      <td>
        <p>As high as desired, depending on the forgetting index.</p>
      </td>
      <td>
        <p>Low, you will forget as soon as you stop using your knowledge.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          <em>Frequency of learning</em>
        </p>
      </td>
      <td>
        <p>As frequent as desired<sup><b>**</b></sup>.</p>
      </td>
      <td>
        <p>Arbitrary or random.</p>
      </td>
    </tr>
  </tbody>
</table>

> **^\*^**: [Piotr Wozniak](/supermemo/piotr-wozniak) executed **spaced repetition on paper** for years before writing the first computer version with SuperMemo, read [his article](https://supermemo.guru/wiki/First_steps_of_SuperMemo#SuperMemo_on_paper).
> 
> **^\*\*^**: Missing out a few days is not the end of the world, but it will require more work later on!
{.is-info}