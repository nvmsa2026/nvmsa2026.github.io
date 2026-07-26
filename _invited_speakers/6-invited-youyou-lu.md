---
name: Youyou Lu
title: Associate Professor
affiliation: Tsinghua University
link: http://storage.cs.tsinghua.edu.cn/~lu/
session: distinguished-invited-session
invited_session: true
priority: 2
talk_time: "15:55 - 16:30"
talk_title: "SuperInfer: Enabling High-Performance Inference for SuperPods"
---
**Abstract**: SuperPod has emerged as a promising infrastructure paradigm for AI training and inference. It provides high-bandwidth interconnected memory, including both GPU memory and host memory. However, how to utilize the hardware performance remains a major challenge. In this talk, I will extend our prior research on disaggregated memory to the domain of disaggregated GPU memory, and present our ongoing work on SuperInfer, a fundamental system layer for high-performance inference engines on SuperPods. Specifically, I will cover three key technical contributions: 1) Morpheral Kernel, a novel abstraction that enables GPU kernels to dynamically yield and reclaim compute resources at runtime. 2) KV Cache management over disaggregated GPU memory and SuperFS, achieving both high performance and low cost. 3) GCR, a GPU checkpoint and restart mechanism to support fault tolerance, cross-device task migration, and dynamic model switching.

**Bio**: Youyou Lu is an associate professor in the Department of Computer Science and Technology at Tsinghua University. He is also the director of Tsinghua University (DCST) - iSoftStone Computer Joint Research Center for Artificial Intelligence Systems. His current research focuses on storage systems and artificial intelligence systems. He serves as PIs for several national major research projects. His research has received multiple awards, including NVMSA'14 Best Paper Award, MSST'15 Best Paper Runner-up, ACM SIGMOD'23 Research Highlight Award, Communications of the ACM'25 Research Highlight, FAST'26 Distinguished Artifact Award, and FAST'26 Best Paper Candidate. He leads the SuperFS file system project, which is deployed in Pengcheng Cloudbrain II and ranked first in the IO500 list from 2023 to 2025. His group also won the 1st place in 2025 ASPLOS/EuroSys and 2026 MLSys LLM inference optimization competition. He is/was on the program committee of different conferences, including FAST, SOSP, OSDI, ATC, EuroSys, NSDI, ASPLOS, etc.
