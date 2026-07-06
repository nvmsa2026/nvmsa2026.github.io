---
author: Han Yan, Dingcui Yu, Yanyun Wang, Yina Lv, Tianyu Ren and Liang Shi.
title: "RARO: Reliability-Aware Read Optimization for Hybrid Flash Storage"
oral: yes
number: 32
---
**Abstract**: Hybrid flash storage combines large-capacity high-density flash memory with high-performance low-density flash memory, providing excellent cost-effectiveness. Existing data placement strategies for hybrid flash storage typically employ hotness-based data migration relying on a two-tier architecture.

This approach not only overlooks the variations in read retry counts across different reliability stages, but also leads to severe capacity degradation and exacerbated write amplification. To address these issues, we propose RARO, a Reliability-Aware Read performance Optimization scheme for hybrid flash storage. RARO redesigns data placement by leveraging application-level data access patterns and device-level flash reliability. This is achieved by dynamically migrating data based on its retry count and access hotness. Data residing in an unsuitable flash type triggers immediate migration, with higher priority given to data exhibiting both high retry counts and hotness for placement into low-density flash, thereby enabling proactive performance optimization. Furthermore, RARO employs a progressive three-tier (SLC-TLC-QLC) management framework to mitigating the capacity loss. The evaluation of RARO, conducted on the FEMU-based emulator, significantly enhances read performance, with IOPS reaching 9.46× to 15.9× of the baseline across different aging stages, while also recovering 57% to 92% of the usable device capacity.
