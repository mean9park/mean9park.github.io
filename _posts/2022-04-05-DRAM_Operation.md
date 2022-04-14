---
layout: single
title: "DRAM Device Configuration"
description: DRAM Structure
date: "2022-04-05 21:12:00 +0900"
last_modified_at: "2022-04-13 21:30:00 +0900"
tags: ["DRAM", "Memory Architecture"]
---
	
> __Part I__ DRAM Device Configuration
---

# DRAM
# (Dynamically Random Access Memory)
is most widely used as a main memory these days.
With a tremendous development of semiconductor industry, the performance of DRAM wouldn't stop. (there's always been people who think the performance is close to an end tho)
How has it been possible to constantly increase the performance?

Well, I guess we first should dive into the details of what DRAM looks like inside and see how it operates.

---

I drew some overall DRAM structure here.
It's one of DDR3 architectures (there are several SPECs), and now we're about to have DDR5, then why DDR3?

DDR4 and DDR5 has been released by addressing some shortcomings of their previous models. 
It even goes far as to say that recent DRAM runs with a combination of thousands techniques, not a single principle.
Before deeply delving into a recent model, I think DDR3 has (or DDR2, DDR1) a basic structure to easily understand "How DRAM operates".

![DRAM_Overall](../assets/images/DRAM_Overall.png)

Messy! Start with the basic (physically smallest) part, DRAM cell.
