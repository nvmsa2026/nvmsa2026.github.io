---
author: Yuquan Chi, Yinjin Fu and Nong Xiao.
title: "PMDangNull: Preventing Use-After-Free for Persistent Memory Applications"
oral: yes
number: 27
---
**Abstract**: Use-after-free (UAF) remains one of the most critical security threats affecting C/C++ programs. Moreover, the cross-restart persistence semantics of persistent memory (PM) programming models significantly broaden the UAF attack surface. Existing DRAM-based protection schemes lack crash consistency guarantees, whereas existing PM-specific solution, which is based on ASan, suffer from high runtime overhead and offers incomplete protection against UAF. In this paper, we present PMDangNull, a collaborative compiler-allocator protection framework built atop LLVM. PMDangNull instruments protected applications with escape-tracking instructions via a compiler plugin, coordinating with its allocator runtime module to enforce pointer nullification upon deallocation. Experimental results under single-threaded execution with no compiler optimization demonstrate that, compared with the existing solution SafePM, PMDangNull reduces performance and space overheads by up to 62.46% and 41.83%, respectively, and successfully prevents all eight UAF exploits in our test suite.
