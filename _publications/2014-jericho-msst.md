---
title: "Jericho: Achieving Scalability Through Optimal Data Placement on Multicore Systems"
collection: publications
permalink: /publication/2014-jericho-msst
excerpt: ' '
date: 2014-06-02
venue: 'International Conference on Massive Storage Systems and Technology (MSST)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/6855538'
citation: ' '
---
Abstract
====
Achieving high I/O throughput on modern servers presents significant challenges. With increasing core counts, server memory architectures become less uniform, both in terms of latency as well as bandwidth. In particular, the bandwidth of the interconnect among NUMA nodes is limited compared to local memory bandwidth. Moreover, interconnect congestion and contention introduce additional latency on remote accesses. These challenges severely limit the maximum achievable storage throughput and IOPS rate. Therefore, data and thread placement are critical for data-intensive applications running on NUMA architectures. In this paper we present Jericho, a new I/O stack for the Linux kernel that improves affinity between application threads, kernel threads, and buffers in the storage I/O path. Jericho consists of a NUMA-aware filesystem and a DRAM cache organized in slices mapped to NUMA nodes. The Jericho filesystem implements our task placement policy by dynamically migrating application threads that issue I/Os based on the location of the corresponding I/O buffers. The Jericho DRAM I/O cache, a replacement for the Linux page-cache, splits buffer memory in slices, and uses per-slice kernel I/O threads for I/O request processing. Our evaluation shows that running the FIO microbenchmark on a modern 64-core server with an unmodified Linux kernel results in only 5% of the memory accesses being served by local memory. With Jericho, more than 95% of accesses become local, with a corresponding 2x performance improvement.

**Recommended citation**: Mavridis, Stelios, Yannis Sfakianakis, Anastasios Papagiannis, Manolis Marazakis, and Angelos Bilas. "Jericho: Achieving scalability through optimal data placement on multicore systems." In <i>Mass Storage Systems and Technologies (MSST)</i>, 2014 30th Symposium on, pp. 1-10. IEEE, 2014.
