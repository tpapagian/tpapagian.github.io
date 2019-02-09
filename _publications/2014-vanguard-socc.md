---
title: "Vanguard: Increasing Server Efficiency via Workload Isolation in the Storage I/O Path."
collection: publications
permalink: /publication/2014-vanguard-socc
excerpt: ' '
date: 2014-11-03
venue: 'ACM Symposium on Cloud Computing (SoCC)'
paperurl: 'https://dl.acm.org/citation.cfm?id=2670998'
citation: ' '
---
Abstract
====
Server consolidation via virtualization is an essential technique for improving infrastructure cost in modern datacenters. From the viewpoint of datacenter operators, consolidation offers compelling advantages by reducing the number of physical servers, and reducing operational costs such as energy consumption. However, performance interference between co-located workloads can be crippling. Conservatively, and at significant cost, datacenter operators are forced to keep physical servers at low utilization levels (typically below 20%), to minimize adverse performance interactions.

In this paper, we focus on addressing the issue of performance interference on a virtualized server operating at high utilization levels. In our work, we find that eliminating interference in the I/O path is critical for achieving good performance on consolidated servers. We present Vanguard, a device driver stack that implements a full I/O path in the Linux kernel that provisions competing workloads with dedicated resources. We focus on two key resources: in-memory buffers for the filesystem, and space on SSD devices that serve as a transparent cache for block devices. Our approach effectively mitigates performance interference, for several mixes of transactional, streaming, and analytical processing workloads. We find that with our approach a server can run more workloads close to their nominal performance level as compared to the unmodified Linux I/O path, by careful allocation of I/O path resources to each workload. At excessive load levels, i.e. when the aggregate load exceeds the capabilities of the server, our approach can still provide isolated slices of the I/O path for a subset of the co-located workloads yielding at least 50% of their nominal performance. In addition, Vanguard is shown to be 2.5x more efficient in terms of service resource usage for a 4-workload mix, taking into account utilization and power consumption. With an I/O-heavy mix 6-workload mix, Vanguard is 8x more efficient than the unmodified baseline Linux system.

**Recommended citation**: Sfakianakis, Yannis, Stelios Mavridis, Anastasios Papagiannis, Spyridon Papageorgiou, Markos Fountoulakis, Manolis Marazakis, and Angelos Bilas. "Vanguard: Increasing server efficiency via workload isolation in the storage i/o path." In <i>Proceedings of the ACM symposium on cloud computing</i>, pp. 1-13. ACM, 2014.
