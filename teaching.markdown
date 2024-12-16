---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: Teaching
permalink: /teaching/
list_title: ' '
---
<link rel="icon" href="{{ "./favicon-32x32.png" | relative_url }}" type="image/x-icon">

<h2> Thesis Supervision </h2>
I am looking for students to supervise (MSc) that are interested in storage systems. I have topics regarding NVMe, performance analysis, QoS tracing, LSM-trees, and storage/network schedulers.
If you are interested please contact me on my mail or join one of our weekly StoNet-research meetings on <a href="https://stonet-research.github.io/index.html">Tuesday 16:00</a>. I am also available in a number of our AtLarge training sessions. For example, I am part of the weekly AtLarge groupmeetings (open to everyone at the VU), and the weekly AtLarge BSc thesis meetings (I am part of their organization, they start around yearly at March/April).

I have co-supervised the following projects:
<ul>
    <li> [BSc HP project] Gleb Mischenko — TBD — WIP </li>
    <li> [MSc thesis] <a href="https://medium.com/@appsby12">Sudarsan Sivakumar</a> — <i>Performance Characterization Study of NVMe Storage Over TCP</i> — <a href="{{ site.url }}/downloads/supervised_thesis_sudarsan_sivakumar_NVMeoFTCP.pdf" style="color:#009988">PDF</a> <a href="https://github.com/stonet-research/NVMeoFTCP-Characterization" style="color:#009988">Code</a> — 2024 </li>
    <li> [BSc thesis] Darko Vujica — <i>Exploring Redis Persistence Modes: Introducing AOFURing, an io_uring AOF Extension</i> —  <a href="{{ site.url }}/downloads/supervised_thesis_darko_vujica_aofuring.pdf" style="color:#009988">PDF</a> <a href="https://github.com/daraccrafter/Thesis-Redis-IO_Uring" style="color:#009988">Code</a> — 2024 </li>
    <li> [BSc thesis] Vincent Kohm — <i>Optimizing Metadata Handling with vkFS: A Hybrid Key-Value Store File System leveraging RocksDB</i> — <a href="{{ site.url }}/downloads/supervised_thesis_vincent_kohm_vkfs.pdf" style="color:#009988">PDF</a> <a href="https://github.com/Vincent881909/vkfs" style="color:#009988">Code</a> — 2024 </li>
    <li> [MSc survey] <a href="https://medium.com/@appsby12">Sudarsan Sivakumar</a> — <i>A survey on flash storage disaggregation: performance and quality of service considerations</i> — <a href="{{ site.url }}/downloads/supervised_survey_sudarsan_sivakumar_flash_storage_disaggregation_qos.pdf" style="color:#009988">PDF</a> —  2024 </li>
</ul>

<h2> Courses </h2>
For my PhD, I have been involved as a teaching assistant (along with coordinating roles) for the following courses:
<ul>
    <li> [2023] — <a href="https://atlarge-research.com/courses/storage-systems-vu/"> Storage Systems (MSc)</a>: StoNet's flagship course. Here we teach students how to design, implement and evaluate storage systems. Students implement an FTL, a GC algorithm and an FS for the NVMe ZNS interface. I was a lead TA and I had roles related to coordination, grading, interviewing students, maintaining the grading/competition framework, server provisioning, lab practicals, student contact person, and I provided educational material for KV-stores.</li>
    <li> [2024] — <a href="https://atlarge-research.com/courses/distr-sys-vu/"> Distributed Systems (MSc)</a>: Teaching students how to design, implement, and evaluate distributed systems. Students can pick a project that aligns with their interest, I gave storage systems related projects to several groups.</li>
    <li> [2023–2024] — <a href="https://atlarge-research.com/courses/advanced-net-prog-vu/2"> Advanced Network Programming (BSc)</a>: Teaching students how to design, implement and evaluate network stacks. Among others they implement ICMP and TCP in user-space for Linux. I was the lead TA for this course, leading the other TAs. I had coordination, grading, interviewer, lab practical, and contact person roles.</li>
    <li> [2023–2025] — <a href="https://research.vu.nl/en/courses/systems-seminar-2"> System Seminar (MSc)</a>: Teaching students how to read <i>and</i> review systems papers. Topics change yearly and we have covered topics ranging from storage, networks, accelerators, programming languages to data center carbon footprint. Additionally, students are given the opportunity to reproduce systems artifacts and write a system artifact review. I have responsibilities regarding the lab practicals, the system artifacts, and grading the reviews.</li>
</ul>

<h2> Academic service </h2>
I have reviewed conference papers from CCGRID, and ICPE, and system artifacts from SOSP.
