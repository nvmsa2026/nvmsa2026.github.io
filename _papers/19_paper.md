---
author: Minki Kang, Bonmoo Koo and Youjip Won.
title: "Understanding the Performance Characteristics of GPUDirect Storage"
poster: yes
number: 9
---
**Abstract**: GPUDirect Storage (GDS) transfers data directly from storage to GPU memory via peer-to-peer DMA, avoiding the host-side copy of the conventional path. Its benefits have been reported mostly in single-threaded settings, leaving its behavior under concurrency unclear.

We characterize GDS and the conventional path as the thread count increases, across a range of I/O sizes. Under small I/O and high concurrency, GDS achieves up to 4x higher throughput (at 192 threads) and roughly 8x less CPU (at 64 threads). GDS thus serves not only to accelerate I/O but also to reduce CPU consumption in concurrent I/O workloads.
