---
author: Haodong Xia, Zhiwei Li, Wenyu Zheng and Liang Shi.
title: "Optimizing Massive Directory Traversal on Portable Flash Storage via Continuity-aware Dynamic Read-Ahead"
oral: yes
number: 34
---
**Abstract**: Portable flash devices, such as TF cards, widely adopt the exFAT file system due to its cross-platform compatibility and support for large-capacity storage. However, directory entries in exFAT exhibit a distributed storage characteristic.

When traversing files within massive small directories, a single read request for a tiny directory entry triggers a large-window read-ahead operation based on physical address alignment. This over-prefetching leads to excessive invalid data reading and storage resource waste, significantly increasing the latency of directory traversal. To address this issue, this paper proposes a continuity-aware dynamic read-ahead scheme. Without altering the file system layout, the proposed scheme dynamically adjusts the read-ahead window by recording the continuity status of historical access sectors in memory. Experimental results demonstrate that this strategy substantially improves the traversal efficiency of massive small directories with negligible overhead, while simultaneously maintaining high sequential read performance for large directories.
