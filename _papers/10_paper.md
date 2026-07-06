---
author: Xiangyu Yao, Yina Lv, Tianyu Ren, Qiao Li and Chun Jason Xue.
title: "Achieving High-Performance Erasure Code Repair through DPU Offloading"
oral: yes
number: 21
---
**Abstract**: Erasure coding provides efficient fault tolerance for large-scale distributed storage systems. However, its data repair process is well-known to be resource-intensive. We find that conventional host-centric, TCP-based repair architectures suffer from severe resource contention. Even in high-bandwidth networks, such interference slows repair operations and degrades service quality. To address this limitation, we propose DPUEC, a novel architecture that fully offloads the entire repair process to a Data Processing Unit (DPU). DPUEC leverages Remote Direct Memory Access (RDMA) to enable kernel-bypass data transfers and utilizes the onboard multi-core processors of DPU for highly parallel decoding. This design establishes a physically isolated data plane for repair traffic, completely bypassing host resources. Our prototype evaluation shows that DPUEC improves repair throughput by 133%–181% over the state-of-the-art approach across different workloads. More importantly, DPUEC delivers true performance isolation. It eliminates any interference with foreground applications and reduces host CPU utilization on the recovery node to nearly zero.
