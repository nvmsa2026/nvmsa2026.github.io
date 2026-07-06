---
author: Jihoon Seok, Juwon Kim and Youjip Won.
title: "LeaST: Learned Sector Translation for Skipped Physical Page Address"
oral: yes
number: 8
---
**Abstract**: In this paper, we propose Learned Sector Translation for Skipped Physical Page Address (LeaST), a mechanism that improves the prediction accuracy of learned-index-based Logical-to-Physical (L2P) mapping by correcting model mis-predictions caused by discontinuities in the physical address space. Learned-index-based L2P mapping relies on the linear correlation between Logical Page Numbers (LPNs) and Physical Page Numbers (PPNs) to accurately predict physical addresses. However, we observe that bad flash pages introduce discontinuities in the physical address space, breaking this linearity, severely degrading prediction accuracy, and consequently deteriorating read performance. LeaST records these discontinuities in a lightweight data structure called the Correction Log and uses it during read operations to correct model-predicted addresses without retraining the model. Compared with LearnedFTL, LeaST improves model prediction accuracy from 11.04% to 93.78%, achieving up to 4.8x higher sequential-read throughput and 1.7x higher random-read throughput.
