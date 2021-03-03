---
title: Urgency-importance Matrix for SuperMemo Tasklists
description: How to boost SuperMemo's tasklist feature by 200%
published: true
date: 2021-03-03T19:31:54.879Z
tags: tasklist
editor: markdown
dateCreated: 2020-12-28T11:47:06.533Z
---

# Urgency-Importance Matrix for SuperMemo Tasklist
> E.T. Jaynes says that reasoning must use all available evidence. By analogy, to get what you want, you should use all available tools. ~ [Mark Xu](https://www.lesswrong.com/s/d922gAtBM8JNzkKKJ/p/yxGBzrGMg4t8QNThA)

Urgency-Importance Matrices, or Eisenhower Matrices, are well known tools for organising tasklists. They are incredibly powerful. 

![urengy-importance_matrix.png](/blogs/squid/urengy-importance_matrix.png)




In SuperMemo, we can replicate this by making four different tasklists for each of the quadrants. I've found this has boosted the quality of my tasklist usage DRAMATICALLY and am never going back.

## Simmplified Values

For additional simplicity, I have also started only using a 1-5 rankng for the values of tasks, making giving tasks a value far simpler and quicker than before.

## Rapid Task Adding
If a task has friction we're less likely to do it. For that reason here's an AutoHotkey script I made that lets you add a task from anywhere with the tap of Alt + Space:

``` 
#IfWinActive

Alt & Space::
WinActivate ahk_class TElWind
send, !{F1}
sleep, 500
send, !s
keywait, Enter, D T10
send, !d
return


```






