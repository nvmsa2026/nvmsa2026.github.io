---
author: Sungjun Yun and Sungyong Ahn.
title: "Near-Data Processing for Homomorphic Ciphertext Operation Offloading over NVMe-oF"
poster: yes
number: 47
---
**Abstract**: Homomorphic encryption (HE) enables direct computation on encrypted data without decryption, but suffers from significant data expansion, whereby a ciphertext can grow up to 1,000 times larger than its plaintext counterparts. This expansion creates a severe I/O bottleneck during data movement between storage and main memory for host-side computation. To address this, Near-Data Processing (NDP), a scheme for processing data near the storage unit, has emerged as one of the promising solutions to reduce the I/O-related overhead. In this paper, we leverage a Storage Performance Development Kit (SPDK) based NDP platform to offload core operations of the CKKS HE scheme. Experimental results demonstrate that compared to the non-offloading baseline, the I/O traffic was reduced by about 99%, and the execution time was decreased by about 28%.
