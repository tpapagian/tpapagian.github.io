---
title: "User-Space I/O for μs-level Storage Devices"
collection: publications
permalink: /publication/2016-iris-wopsss
excerpt: ' '
date: 2016-06-19
venue: 'High Performance Computing: ISC High Performance 2016 International Workshops, ExaComm, E-MuCoCoS, HPC-IODC, IXPUG, IWOPH, P^3MA, VHPC, WOPSS, Revised Selected Papers'
paperurl: 'https://link.springer.com/chapter/10.1007/978-3-319-46079-6_44'
citation: ' '
---
Abstract
====
System software overheads in the I/O path, including VFS and file system code, become more pronounced with emerging low-latency storage devices. Currently, these overheads constitute the main bottleneck in the I/O path and they limit efficiency of modern storage systems. In this paper we present Iris, a new I/O path for applications, that minimizes overheads from system software in the common I/O path. The main idea is the separation of the control and data planes. The control plane consists of an unmodified Linux kernel and is responsible for handling data plane initialization and the normal processing path through the kernel for non-file related operations. The data plane is a lightweight mechanism to provide direct access to storage devices with minimum overheads and without sacrificing strong protection semantics. Iris requires neither hardware support from the storage devices nor changes in user applications. We evaluate our early prototype and we find that it achieves on a single core up to   1.7×  and   2.2×  better read and write random IOPS, respectively, compared to the xfs and ext4 file systems. It also scales with the number of cores; using 4 cores Iris achieves   1.84×  and   1.96×  better read and write random IOPS, respectively.

**Recommended citation**: Anastasios Papagiannis, Giorgos Saloustros, Manolis Marazakis, and Angelos Bilas. "User-space I/O for μs-level storage devices." In <i>High Performance Computing: ISC High Performance 2016 International Workshops, ExaComm, E-MuCoCoS, HPC-IODC, IXPUG, IWOPH, P^3MA, VHPC, WOPSSS</i>, Frankfurt, Germany, June 19-23, 2016, Revised Selected Papers, Springer International Publishing.
