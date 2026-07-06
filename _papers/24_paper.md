---
author: Euihyeon Kim and Sungyong Ahn.
title: "Acceleration of RAG Pipeline with NVMe-oF based Near-Data Processing for Edge LLM Inference"
poster: yes
number: 46
---
**Abstract**: Retrieval-augmented generation (RAG) has become a critical technique for LLM service, as it reduces hallucinations and enables up-to-date LLM response, but deploying it on resource-constrained edge devices is challenging, as the vector DB required for retrieval often resides on a remote storage server, causing substantial data movement across the fabric. We propose offloading the entire RAG pipeline to an NVMe-oF-based storage server, returning only the resulting token sequence to the edge. On a Jetson Orin Nano prototype over NVMe-oF/TCP, this reduces edge–server data movement by roughly 95% compared to a baseline that retrieves over the fabric.
