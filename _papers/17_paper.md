---
author: Yongqing Huang, Yangchun Gong, Jian Chen, Yina Lv and Congming Gao.
title: "ROSS: A Cross-Layer Network-and-SSD Simulator for NVMe over RDMA Target Offload"
oral: yes
number: 44
---
**Abstract**: NVMe over Fabrics (NVMe-oF) over RDMA target offload is an important architecture for high-performance disaggregated storage systems. By moving target-side NVMe-oF processing into RDMA-capable NICs or DPUs, target offload reduces host CPU involvement and enables efficient data movement between the network and backend NVMe SSDs. However, the involved I/O path spans host-side request submission, RDMA transport, target-side offload admission, PCIe/DMA movement, and SSD internal execution, making it difficult for network-only or SSD-only simulators to capture its end-to-end behavior.

This paper presents ROSS, a cross-layer network-and-SSD simulator for NVMe-oF over RDMA target offload. ROSS extends an ns-3 RDMA frontend with host-memory RDMA queue modeling, RNIC WQE-fetch delay, target-side eXtended Receive Queue (XRQ) admission, Receiver Not Ready (RNR)-triggered retry, and RNIC-offloaded data movement. It further couples ns-3 with MQSim to model backend NVMe SSD execution under a unified event-driven timeline. We validate ROSS against a real NVMe-oF over RDMA target offload testbed using read and write workloads with I/O sizes varying from 4 KB to 1024 KB. Compared with real hardware measurements, ROSS captures the overall latency and bandwidth trends with an average performance error of 7.97%.
