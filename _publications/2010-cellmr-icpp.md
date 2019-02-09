---
title: "Rearchitecting mapreduce for heterogeneous multicore processors with explicitly managed memories"
collection: publications
permalink: /publication/2010-cellmr-icpp
excerpt: ' '
date: 2010-09-13
venue: 'International Conference on Parallel Processing (ICPP)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/5599156'
citation: ' '
---
Abstract
====
This paper presents a new design and an implementation of the runtime system of MapReduce for heterogeneous multicore processors with explicitly managed local memories. We advance the state of the art in runtime support for MapReduce using five instruments: (1) A new multi-threaded, event-driven controller for task instantiation, task scheduling, synchronization, and bulk-synchronous execution of MapReduce stages. The controller improves utilization of control efficient cores, minimizes control overhead in the runtime system, and overlaps task instantiation with task scheduling on compute-efficient cores. (2) An implicit partitioning scheme which eliminates redundant memory copies. (3) An adaptive memory management scheme which combines efficient memory preallocation for applications with statically known output volume with dynamic allocation using runahead tasks for applications with statically unknown output volume. (4) An optimized quick-sort/merge-sort scheme which reduces the critical path length of merge-sort. (5) An optimized execution scheme which avoids redundant data transfers to and from local stores in applications that emit keys with the same value. Put together, these techniques accelerate representative MapReduce workloads by a factor of 1.81x (geometric mean) compared to a reference design that represents the state of the art.

**Recommended citation**: Papagiannis, Anastasios, and Dimitrios S. Nikolopoulos. "Rearchitecting mapreduce for heterogeneous multicore processors with explicitly managed memories." In <i>Parallel Processing (ICPP), 2010 39th International Conference on</i>, pp. 121-130. IEEE, 2010.

