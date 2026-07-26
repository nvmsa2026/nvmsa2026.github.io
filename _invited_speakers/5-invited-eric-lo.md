---
name: Eric Lo
title: Associate Professor
affiliation: The Chinese University of Hong Kong
link: https://www.cse.cuhk.edu.hk/people/faculty/eric-chi-lik-lo/
session: distinguished-invited-session
invited_session: true
priority: 1
talk_time: "15:20 - 15:55"
talk_title: "High-performance Deployment Stack for Disaggregated Memory Indexing"
---
**Abstract**: Disaggregated memory, enabled by high-speed interconnects such as RDMA and emerging CXL, is rapidly becoming a key building block for next-generation data centers. While this architecture promises flexible resource pooling and improved utilization, achieving high performance in fundamental indexing structures (e.g., B+ trees and hash tables) on disaggregated memory today still demands deep, manual co-design of data structures and hardware, extensive code refactoring, and careful handling of cache and consistency issues across multi-threaded remote memory accesses. In practice, only a handful of expert-crafted indices can fully exploit these platforms, creating a high barrier to adoption.

In this talk, I will present Penthalon, a high-performance deployment stack that automates the specialization of battle-tested multi-threaded index implementations for disaggregated memory systems. Penthalon consists of a compiler and a remote runtime that together take an existing, well-engineered index as input and produce an optimized binary that runs efficiently on a given RDMA/CXL-based disaggregated memory platform, without requiring changes to the original index code. Our evaluation shows that, for B+ trees, Penthalon can transform ordinary implementations to outperform human-optimized indices such as Sherman (SIGMOD'22), and to approach the performance of DEX (VLDB'24). Similarly, for hash tables, Penthalon turns standard implementations into deployments that surpass SepHash (VLDB'24) and come close to Shard (VLDB'25), all while reducing manual optimization and coding effort to essentially zero. The talk will conclude with lessons learned about disaggregated memory-aware indexing and how automated deployment stacks can reshape the way systems researchers and practitioners approach index design in this emerging landscape.

**Bio**: Eric Lo is currently an Associate Professor of Computer Science and Engineering at the Chinese University of Hong Kong (CUHK). He earned his PhD from ETH Zurich and has previously worked at both Google and Microsoft. His recent research focuses on emerging memory, serving systems for AI agents, and cloud databases. He is currently the PC Chair for ACM SoCC '26 and an Associate Editor for both PVLDB and The VLDB Journal. His work has received recognition through awards and honorable mentions at conferences such as VLDB 2005 and ICDE 2012. In 2020, he was awarded the ACM SIGMOD Research Highlight Award.
