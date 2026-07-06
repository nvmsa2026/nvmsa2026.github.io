---
author: Zelin Du and Zili Shao.
title: "Rethinking SSD Firmware Scalability with Data First Commit Later Principle"
poster: yes
number: 16
---
**Abstract**: Modern SSD firmware often suffers from blocking execution paths, where flash I/O, cache updates, and metadata commits are tightly coupled. This paper proposes a Data First, Commit Later pipeline design that decouples data movement from state commitment. Flash I/O is issued first, while Data Cache updates and commit operations are deferred until consistency constraints are satisfied.

We further develop a latency and throughput model for pipelined SSD firmware, showing that the Flash Interface Layer (FIL) can become the dominant bottleneck when NAND resources are underutilized. Based on this observation, we introduce an out-of-order FIL waiting-list scheduler that issues dependency-free flash transactions in die-level read/write streams according to NAND resource availability, further improving backend bandwidth utilization.
