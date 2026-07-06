---
author: Can Gao, Xuejin Li and Keni Qiu.
title: "A Bipartite-graph Guided DNN Weight Remapping Scheme for Achieving Low-cost MRAM CIM Reprogramming"
oral: yes
number: 12
---
**Abstract**: Compute-in-memory (CIM) architectures mitigate the von-Neumann bottleneck by embedding computation directly within memory crossbars, delivering order-of-magnitude improvements in energy efficiency and throughput. Among the emerging technologies, non-volatile-memory (NVM)-based CIM is particularly attractive owing to its non-volatility, ultra-low standby power, and high integration density. Nevertheless, capacity-constrained NVM crossbars can accommodate only a fraction of a deep neural network’s weights at any instant, necessitating frequent reprogramming that incurs substantial latency and energy penalties. We observe that the problem of scheduling weight updates onto such a limited-capacity crossbar is isomorphic to a bipartite-graph assignment problem.

Motivated by this insight, we propose a static scheduling framework that systematically minimizes reprogramming cost. The framework comprises three synergistic stages: (i) bipartite-graph–driven row- and column-reordering formulated as an optimal assignment problem; (ii) fine-grained bit-flip minimization guided by hardware-aware correction logic; and (iii) a priority-driven consolidation layer that allows designers to favor either energy or latency. Evaluations conducted on a customized STT-MRAM CIM simulator demonstrate an average 41% reduction in programming energy, an average 19% reduction in latency, and a 49% improvement in the energy-delay product over the conventional baseline.
