---
title: Incremental Writing
description: 
published: true
date: 2020-12-18T11:27:17.134Z
tags: 
editor: markdown
dateCreated: 2020-12-06T12:18:40.220Z
---

# Incremental Writing

**Incremental Writing (IW)** is a method for boosting creativity, quality and pleasure of writing. It synergizes with the natural ability of your brain to update knowledge and organize it into concept networks.

Incremental writing is an extension of [incremental reading](/learning/incremental-reading). You should be familiar with it before considering incremental writing.

## How does it work ?

Incremental writing is typically assisted by software to maximize the usage of your time by interspacing:

- Reviewing new learning material to develop new insights, 
- Reviewing previously acquired knowledge to preserve it over time (forever !), 
- Creative work (writing, problem solving, ...).

In IW, the decision of whether you should continue working on a particular text depends on your desire to do so. That desire is a compound of variables: [pleasure of writing](/reference-manual/pleasure-of-learning), state of flow, level of understanding of the topic, etc.

```mermaid

graph TB
  step1{{"New article (next repetition)"}}:::state
  
  subgraph IR[" "]
    IR-step1["Do Incremental Reading"]:::type
    IR-step2>"Read article"]
    IR-step3("<img src='/supermemo/incremental-reading/ir-1st-rep-step-1.png'; width='250px' height='154px'/>")
    IR-step4["Acquire knowledge"]
  end
  
  subgraph IW[" "]
    IW-step1["Do Incremental Writing"]:::type
    IW-step2-a["Update content using new knowledge"]
    IW-step2-b["Add new content"]
    IW-step3["Consolidate knowledge"]
  end
  
  
  step1                   -. If writing article                 -..-> IW-step1
  IW-step1                -- 1.a. Read and locate mistakes        --> IW-step2-a
  IW-step1                -- 1.b. New ideas                       --> IW-step2-b
  IW-step2-a & IW-step2-b                                         --> IW-step3
  IW-step3                -- 2. Repeat until bored                --> IW-step1
  IW-step3                -. 3. When bored with current article   .-> step1
  
  
  step1                   -. If learning article                       -.-> IR-step1
  IR-step1                                                              --> IR-step2
  IR-step2                -- 1. Locate interesting information          --> IR-step3
  IR-step3                -- 2. Extract valuable text for later         --> IR-step4
  IR-step4                -- 3. Repeat until bored with current article --> IR-step2
  IR-step4                -. 4. When bored with current article         .-> step1
  
  classDef state fill:#F3FFDA,stroke-width:2px
  classDef type fill:#72F87C,color:#333
```

## Benefits

A typical incremental writer:

- Never gets bored (there are always new and varied ideas to keep things exciting), 
- Increases his creativity (new information is constantly flowing), 
- Writes more efficiently (by progressing on several sections in parallel), 
- Is less prone to error (dividing in smaller sections makes it easier to spot mistakes, and update erroneous or outdated information with new understandings).
