---
title: SuperMemo Queues
description: Queues are ways of ordering material yet to be reviewed.
published: true
date: 2020-12-13T08:35:41.420Z
tags: 
editor: markdown
dateCreated: 2020-12-13T08:35:41.420Z
---

# What are Queues?

If you use [SuperMemo](/supermemo) long enough, your [collection](https://supermemo.guru/wiki/Collection) will grow to contain thousands of pieces of knowledge. They are called **elements**.

The multiplicity of material calls for a questions: in which order should I process each individual element? To address that question, SuperMemo implements **queues**: a set of elements ordered according to some criteria (e.g. priority, randomness, etc.)

```mermaid

graph LR
  el1["<img src='/supermemo/shared/article-ex-1-circardian-rhythm.png'; width='150px' height='186px'/>"]
  el2["<img src='/supermemo/shared/article-ex-2-lti.png'; width='150px' height='141px'/>"]
  el3["<img src='/supermemo/shared/article-ex-3-anthropology.png'; width='150px' height='211px'/>"]
  
  el1 --> el2
  el2 --> el3
  el3 --> others
```