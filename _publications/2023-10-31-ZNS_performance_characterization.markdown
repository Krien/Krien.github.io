---
layout: post
title: "Performance Characterization of NVMe Flash Devices with Zoned Namespaces (ZNS)"
date:  2023-10-31
authors: 
    - "Krijn Doekemeijer"
    - "Nick Tehrany"
    - "Balakrishnan Chandrasekaran"
    - "Matias  Bjørling"
    - "Animesh Trivedi"
categories: flash "performance characterization" ZNS
short: "A performance characterization of the ZNS interface)"
status: Done
conference: "2023 IEEE International Conference on Cluster Computing (CLUSTER)"
type: conference
selected: yes
other: ""
---

<h2>Abstract</h2>
e recent emergence of NVMe flash devices with Zoned Namespace support, ZNS SSDs, represents a significant
new advancement in flash storage. ZNS SSDs introduce a new storage abstraction of append-only zones with a set of new I/O
(i.e., append) and management (zone state machine transition) commands. With the new abstraction and commands, ZNS SSDs
offer more control to the host software stack than a non-zoned SSD for flash management, which is known to be complex
(because of garbage collection, scheduling, block allocation, parallelism management, overprovisioning). ZNS SSDs are, consequently,
gaining adoption in a variety of applications (e.g., file systems, key-value stores, and databases), particularly latency-
sensitive big-data applications. Despite this enthusiasm, there has yet to be a systematic characterization of ZNS SSD performance
with its zoned storage model abstractions and I/O operations. This work addresses this crucial shortcoming. We report on the
performance features of a commercially available ZNS SSD (13 key observations), explain how these features can be incorporated
into publicly available state-of-the-art ZNS emulators, and recommend guidelines for ZNS SSD application developers.
All artifacts (code and data sets) of this study are publicly available at [https://github.com/stonet-research/NVMeBenchmarks](https://github.com/stonet-research/NVMeBenchmarks).

<h2>Metadata</h2>
- <b>Authors:</b> Krijn Doekemeijer, Nick Tehrany, Balakrishnan Chandrasekaran, Matias  Bjørling, Animesh Trivedi
- <b>Type:</b> Conference paper
- <b>Keywords:</b> Measurements, NVMe storage, Zoned Namespace Devices
- <b>Publish date:</b> 2023-10-31

<h2>Availability</h2>
- Paper at AtLarge: [2023-cluster-zns-performance-kdoekemeijer.pdf](https://atlarge-research.com/pdfs/2023-cluster-zns-performance-kdoekemeijer.pdf).
- Paper at IEEE: [https://ieeexplore.ieee.org/document/10319951](https://ieeexplore.ieee.org/document/10319951f).
- Code: [https://github.com/stonet-research/NVMeBenchmarks](https://github.com/stonet-research/NVMeBenchmarks).
