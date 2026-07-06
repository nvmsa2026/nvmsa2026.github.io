---
author: Lei Li, Riwei Pan and Yu Liang.
title: "Reducing Mobile Application Cold-Start Latency via Launch-Critical Data Identification"
outstanding: yes
number: 3
---
**Abstract**: Application cold start is often slowed by page cache misses when launch-critical data must be fetched from flash storage under limited memory capacity. In this paper, we analyze application launch behavior to identify the critical data that most affects launch latency, and refine launch-time measurement to include both activity launch and interface display. Based on this analysis, we propose FLCD, a lightweight mechanism that identifies and retains launch-critical data in memory instead of prefetching all launch-related data. Evaluation on Android smartphones shows that FLCD reduces application launch time by 25\% on average compared to the default Android launch mechanism, with very small memory overhead.
