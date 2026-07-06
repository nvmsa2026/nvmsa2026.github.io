---
author: Junhyeok Jeong and Jaeho Kim
title: "SAF: Semantic-Aware Flushing for Latency and Jitter Suppression in Continuous VLA Inference on Edge Devices	"
poster: yes
number: 39
---
**Abstract**: In memory-constrained edge devices, continuous Vision-Language-Action inference, where KV caches are offloaded via mmap to NVMe, often exhibits high tail latency and jitter. The main reason for this is that OS background flushers, such as pdflush/kworker, are not aware of the timing of inference. This can result in bursty writeback I/O during execution, which interferes with real-time control.

To address this issue, we propose Semantic-Aware Flushing (SAF). SAF detects the semantic boundaries of frame responses and actively flushes dirty pages during the inter-frame idle interval. This reduces the interference between inference and storage I/O.

We evaluate four flush policies using Moondream2 on Jetson Orin NX, with flush timing controlled via OS parameters or application-level triggers. The results show that SAF reduced the average latency by 24.2%, from 9,804 ms to 7,427 ms.

Similarly, P99 tail latency decreased by 27.7%, from 16,174 ms, to 11,696 ms, and jitter(IQR) decreased by 77.8%, from 2,893 ms to 642 ms. In addition, SAF also eliminated all 295 OS flusher interventions associated with the default policy.
