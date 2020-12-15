---
title: SuperMemo Queues
description: Queues are ways of ordering material yet to be reviewed.
published: true
date: 2020-12-13T09:36:25.410Z
tags: 
editor: markdown
dateCreated: 2020-12-13T08:35:41.420Z
---

# What are Queues?

If you use [SuperMemo](/supermemo) long enough, your [collection](https://supermemo.guru/wiki/Collection) will grow to contain thousands of pieces of knowledge. They are called **elements**.

The multiplicity of material calls for a question: in which order should I process each individual element? To address that issue, SuperMemo implements **queues**: a set of elements ordered according to some criteria (e.g. [priority](/supermemo/priority), randomness, etc.)

For the rest of this article we will use the example below, three articles: Circadian rhythm, LTI and Anthropology.

```mermaid

graph TB
  el1["<img src='/supermemo/shared/article-ex-1-circardian-rhythm.png'; width='150px' height='186px'/>"]
  el2["<img src='/supermemo/shared/article-ex-2-lti.png'; width='150px' height='141px'/>"]
  el3["<img src='/supermemo/shared/article-ex-3-anthropology.png'; width='150px' height='211px'/>"]
  
```

## Priority queue

The **priority queue** contains all the elements ordered by priority. [Priorities](/supermemo/priority) are defined from 0% to 100%, with 0% being the most prioritized, and 100% the least prioritized. In our example, let's assume the following priorities:
| Priorities                               |||
| Circadian rhythm |   LTI    | Anthropology |
|:================:|:========:|:============:|
| **5%**           | **75%** | **30%**      |

The resulting priority queue would be the following:

```mermaid

graph LR
  el1["<img src='/supermemo/shared/article-ex-1-circardian-rhythm.png'; width='150px' height='186px'/>"]
  el2["<img src='/supermemo/shared/article-ex-2-lti.png'; width='150px' height='141px'/>"]
  el3["<img src='/supermemo/shared/article-ex-3-anthropology.png'; width='150px' height='211px'/>"]
  
  el1 --> el3
  el3 --> el2
```

## Outstanding queue

🚧 Work in progress.

## Pending queue

🚧 Work in progress.