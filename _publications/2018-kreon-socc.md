---
title: "An Efficient Memory-Mapped Key-Value Store for Flash Storage."
collection: publications
permalink: /publication/2018-kreon-socc
excerpt: ' '
date: 2018-10-11
venue: 'ACM Symposium on Cloud Computing (SoCC)'
paperurl: 'https://dl.acm.org/citation.cfm?id=3267824'
citation: ' '
---
Abstract
====
Persistent key-value stores have emerged as a main component in the data access path of modern data processing systems. However, they exhibit high CPU and I/O overhead. Today, due to power limitations it is important to reduce CPU overheads for data processing.

In this paper, we propose Kreon, a key-value store that targets servers with flash-based storage, where CPU overhead and I/O amplification are more significant bottlenecks compared to I/O randomness. We first observe that two significant sources of overhead in state-of-the-art key-value stores are: (a) The use of compaction in LSM-Trees that constantly perform merging and sorting of large data segments and (b) the use of an I/O cache to access devices, which incurs overhead even for data that reside in memory. To avoid these, Kreon performs data movement from level to level by performing partial instead of full data reorganization via the use of a full index per-level. In addition, Kreon uses memory-mapped I/O via a custom kernel path with Copy-On-Write.

We implement Kreon as well as our custom memory-mapped I/O path in Linux and we evaluate Kreon using commodity SSDs with both small and large datasets (up to 6 billion keys). For a large dataset that stresses I/O, Kreon reduces CPU cycles/op by up to 5.8x, reduces I/O amplification for inserts by up to 4.61x, and increases insert ops/s by up to 5.3x, compared to RocksDB, a state-of-the-art key-value store that is broadly used today.

**Recommended citation**: Papagiannis, Anastasios, Giorgos Saloustros, Pilar González-Férez, and Angelos Bilas. "An Efficient Memory-Mapped Key-Value Store for Flash Storage." In <i>Proceedings of the ACM Symposium on Cloud Computing</i>, pp. 490-502. ACM, 2018.
