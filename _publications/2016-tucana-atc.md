---
title: "Tucana: Design and Implementation of a Fast and Efficient Scale-up Key-value Store."
collection: publications
permalink: /publication/2016-tucana-atc
excerpt: ' '
date: 2016-06-22
venue: 'USENIX Annual Technical Conference (ATC)'
paperurl: 'https://www.usenix.org/conference/atc16/technical-sessions/presentation/papagiannis'
citation: ' '
---
Abstract
====
Given current technology trends towards fast storage devices and the need for increasing data processing density, it is important to examine key-value store designs that reduce CPU overhead. However, current key-value stores are still designed mostly for hard disk drives (HDDs) that exhibit a large difference between sequential and random access performance, and they incur high CPU overheads.

In this paper we present Tucana, a feature-rich keyvalue store that achieves low CPU overhead. Our design starts from a Be –tree approach to maintain asymptotic properties for inserts and uses three techniques to reduce overheads: copy-on-write, private allocation, and direct device management. In our design we favor choices that reduce overheads compared to sequential device accesses and large I/Os.

We evaluate our approach against RocksDB, a stateof- the-art key-value store, and show that our approach improves CPU efficiency by up to 9:2x and an average of 6x across all workloads we examine. In addition, Tucana improves throughput compared to RocksDB by up to 7x. Then, we use Tucana to replace the storage engine of HBase and compare it to native HBase and Cassandra two of the most popular NoSQL stores. Our results show that Tucana outperforms HBase by up to 8x in CPU efficiency and by up to 10x in throughput. Tucana’s improvements are even higher when compared to Cassandra.

[Download paper here](https://www.usenix.org/system/files/conference/atc16/atc16_paper-papagiannis.pdf)

**Recommended citation**: Papagiannis, Anastasios, Giorgos Saloustros, Pilar González-Férez, and Angelos Bilas. "Tucana: Design and Implementation of a Fast and Efficient Scale-up Key-value Store." In <i>USENIX Annual Technical Conference</i>, pp. 537-550. 2016.
