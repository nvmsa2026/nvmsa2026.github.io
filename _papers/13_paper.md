---
author: Jingcheng Shen, Mingzhe Chen, Linbo Long, Pengju Shui, Congming Gao, Fumihiko Ino and Kenichi Hagihara.
title: "Enhancing I/O Fairness in ZNS SSDs via Multi-Chip Queue Scheduling"
oral: yes
number: 28
---
**Abstract**: The Zoned Namespace (ZNS) interface has emerged as a promising alternative to the traditional block interface for flash-based SSDs. ZNS SSDs divide the logical address space into sequential-write zones. Each zone is mapped across multiple flash chips to enhance intra-zone parallelism. However, this multi-chip mapping intensifies resource contention and degrades I/O access fairness. Existing fairness optimizations, which focus on individual chip queues, exacerbate the slack between cross-chip transactions of a single request, leading to performance loss in multi-flow (e.g., multi-application and multi-tenant) scenarios.

This paper proposes MCFair, a multi-chip fairness scheduling strategy for ZNS SSDs, designed to improve fairness while preserving performance. MCFair integrates three key components: 1) a novel unfairness detector based on a classification algorithm that identifies all unfair I/O flows in real time; 2) a priority-based scheduler that prioritizes unfair flows while adhering to ZNS SSDs' sequential-write constraint; and 3) a slack-aware tuner that minimizes cross-chip slack via transaction alignments. A comprehensive series of experiments based on the FEMU emulator have been conducted, demonstrating that MCFair achieves an average 105.79% fairness improvement and 5.72% response time reduction compared to the baseline. Moreover, compared with state-of-the-art studies FLIN and Fair-ZNS, MCFair improves fairness by 26.77% and 17.89%, and reduces response time by 9.18% and 10.08%, respectively.
