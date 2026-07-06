---
author: Yaotian Cui, Kecheng Huang and Zili Shao.
title: "A Checkpoint-aware Logging Design for Efficient Roll-forward Crash Recovery in F2FS"
oral: yes
number: 23
---
**Abstract**: F2FS (Flash-Friendly File System) has been widely adopted in Android mobile systems, where its roll-forward recovery mechanism plays a pivotal role in ensuring data persistence on mobile devices. However, existing tag-based approaches, which rely heavily on strictly ordered data commits, often fail to achieve reliable data recovery in practical scenarios.

To address this critical limitation, we integrate logging mechanisms into crash recovery and propose a checkpoint-aware logging design specifically tailored for roll-forward recovery. This design eliminates the reliance on tagging and stringent order constraints, instead logging critical semantic information during persistence commands (e.g., fsync). By aligning with the inherent characteristics of flash memory, this approach not only maintains stable runtime performance but also accelerates the recovery process by obviating the need for time-consuming block traversal.

Comprehensive evaluations demonstrate that our proposed design ensures reliable data recovery under power failure scenarios, outperforming traditional systems by up to 83.1% in recovery speed while preserving favorable runtime performance.
