---
layout: single
title: "DRAM Architecture and Operation"
description: DRAM Architecture and Operation
date: "2022-04-05 21:12:00 +0900"
last_modified_at: "2022-04-13 21:30:00 +0900"
tags: ["DRAM", "Memory Architecture"]
---
	
> __Part I__ DRAM Device Configuration
---

# DRAM
# (Dynamic Random Access Memory)
is most widely used as a main memory these days.
With a tremendous development of semiconductor industry, the performance of DRAM has been increasing. (There's always been people who thought it's close to the end tho)
How has it been possible to constantly increase the performance?

Well, I guess we first should dive into what DRAM looks like inside and see how it operates.

---

I drew a "simplified" (plz not be offended by undetailed illustration) version of overall DRAM structure here.
It's one of DDR3 architectures (among several SPECs of DDR3), and now we're about to have DDR5, then why DDR3?

DDR4 and DDR5 have been released by addressing some shortcomings of their previous models, let alone improving the performance. 
The thing is that nowadays DRAMs run with a combination of thousands techniques, not a single operation principle due to a lot of development that's been stacked.
Before deeply delving into a recent DRAM architecture, first looking into DDR3 (or DDR2, DDR1) that has a basic structure would be a good idea to understand "How DRAM operates". 

![DRAM_Overall](../assets/images/DRAM_Overall.png)

Messy! Start with the basic (the smallest) part, __DRAM cell__.

---
<p align="center">
<img src="../assets/images/DRAM_Cell.png" alt="DRAM_Cell" width="300"/>
</p>

This is a basic DRAM Cell (1T1C : 1 transistor & 1 capacitor). Wait here, the basic implies different cell structures like 3T1C, so you can search for them ~~or just click the link if you're curious about [3T1C DRAM Cell.](https://google/com) to be updated soon~~
Again, 
