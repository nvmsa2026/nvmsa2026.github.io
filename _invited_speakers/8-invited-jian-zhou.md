---
name: Jian Zhou
title: Associate Professor
affiliation: Huazhong University of Science and Technology
session: distinguished-invited-session
invited_session: true
priority: 4
talk_time: "17:05 - 17:40"
talk_title: "Hitchhike: Efficient Request Submission via Deferred Enforcement of Address Contiguity"
---
**Abstract**: Modern storage systems operate under high concurrency, making large volumes of outstanding I/Os the norm. However, current I/O submission logic requires requests assigned to the same CPU core to be processed in a serialized manner, turning the software stack into a bottleneck due to high per-request overhead. Hitchhike defers the address contiguity validation to the NVMe device driver, allowing a single request to encapsulate multiple non-contiguous addresses to amortize redundant kernel overhead. It achieves up to 3.5× throughput improvement on single core, cuts the CPU cores needed to saturate NVMe bandwidth by 75%, and maintains full compatibility with standard OS stacks and existing hardware.

**Bio**: Jian Zhou is an associate professor at Wuhan National Laboratory for Optoelectronics, Huazhong University of Science and Technology. He received his Ph.D. in Computer Engineering from the University of Central Florida in 2018, and worked as a postdoctoral researcher there from 2018 to 2020. His research focuses on non-volatile memory, solid-state storage technology, and distributed systems. He has published more than 30 papers in top-tier conferences and journals such as ISCA, SIGMOD, ASPLOS and ATC, and led over a number of national scientific research projects. His research results have been applied in cooperation with leading enterprises to promote industrialization.
