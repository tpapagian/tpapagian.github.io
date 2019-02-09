---
title: "Iris: An optimized I/O stack for low-latency storage devices"
collection: publications
permalink: /publication/2016-iris-osr
excerpt: ' '
date: 2016-12-02
venue: 'ACM SIGOPS Operating Systems Review'
paperurl: 'https://dl.acm.org/citation.cfm?id=3041713'
citation: ' '
---
Abstract
====
System software overheads in the I/O path, including VFS and file system code, become more pronounced with emerging low-latency storage devices. Currently, these overheads constitute the main bottleneck in the I/O path and they limit efficiency of modern storage systems. In this paper we present a taxonomy of the current state-of-the-art systems on accelerating accesses to fast storage devices. Furthermore, we present Iris, a new I/O path for applications, that minimizes overheads from system software in the common I/O path. The main idea is the separation of the control and data planes. The control plane consists of an unmodified Linux kernel and is responsible for handling data plane initialization and the normal processing path through the kernel for non-file related operations. The data plane is a lightweight mechanism to provide direct access to storage devices with minimum overheads and without sacrificing strong protection semantics. Iris requires neither hardware support from the storage devices nor changes in user applications. We evaluate our early prototype and we find that it achieves on a single core up to 1:7x and 2:2x better read and write random IOPS, respectively, compared to the XFS and EXT4 file systems. It also scales with the number of cores; using 4 cores Iris achieves 1:84x and 1:96x better read and write random IOPS, respectively. In sequential reads we provide similar performance and in sequential writes we are about 20% better compared to other file systems.

**Recommended citation**: Papagiannis, Anastasios, Giorgos Saloustros, Manolis Marazakis, and Angelos Bilas. "Iris: An optimized I/O stack for low-latency storage devices."<i>ACM SIGOPS Operating Systems Review 50</i>, no. 2 (2017): 3-11.
