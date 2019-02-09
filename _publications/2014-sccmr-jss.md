---
title: "Hybrid address spaces: A methodology for implementing scalable high-level programming models on non-coherent many-core architectures"
collection: publications
permalink: /publication/2014-sccmr-jss
excerpt: ' '
date: 2014-11-01
venue: 'Journal of Systems and Software, Elsevier'
paperurl: 'https://www.sciencedirect.com/science/article/pii/S0164121214001496'
citation: ' '
---
Abstract
====
This paper introduces hybrid address spaces as a fundamental design methodology for implementing scalable runtime systems on many-core architectures without hardware support for cache coherence. We use hybrid address spaces for an implementation of MapReduce, a programming model for large-scale data processing, and the implementation of a remote memory access (RMA) model. Both implementations are available on the Intel SCC and are portable to similar architectures. We present the design and implementation of HyMR, a MapReduce runtime system whereby different stages and the synchronization operations between them alternate between a distributed memory address space and a shared memory address space, to improve performance and scalability. We compare HyMR to a reference implementation and we find that HyMR improves performance by a factor of 1.71× over a set of representative MapReduce benchmarks. We also compare HyMR with Phoenix++, a state-of-art implementation for systems with hardware-managed cache coherence in terms of scalability and sustained to peak data processing bandwidth, where HyMR demonstrates improvements of a factor of 3.1× and 3.2× respectively. We further evaluate our hybrid remote memory access (HyRMA) programming model and assess its performance to be superior of that of message passing.

**Recommended citation**: Papagiannis, Anastasios, and Dimitrios S. Nikolopoulos. "Hybrid address spaces: A methodology for implementing scalable high-level programming models on non-coherent many-core architectures." <i>Journal of Systems and Software</i> 97 (2014): 47-64.
