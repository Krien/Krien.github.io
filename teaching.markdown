---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: Teaching
permalink: /teaching/
list_title: ' '
---
<link rel="icon" href="{{ "./favicon-32x32.png" | relative_url }}" type="image/x-icon">

<h2> Student Supervision </h2>
<!-- I am looking for students to supervise (MSc) that are interested in storage systems. I have topics regarding NVMe, performance analysis, QoS tracing, and storage/network schedulers.
If you are interested please contact me on my mail or join one of our weekly StoNet-research meetings on <a href="https://stonet-research.github.io/index.html">Tuesday 11:00</a>. I am also available in a number of our AtLarge training sessions. For example, I am part of the weekly AtLarge groupmeetings (open to everyone at the VU). -->

If you are a student, I am unfortunately not currently looking to supervise students. However, feel free to reach out to me with any questions. I also believe in the power of open-sourcing student works. I have supervised projects (BSc and MSc level) on storage system performance characterizations and optimizations.  Students have completed the following projects successfully with me as a daily supervisor at Vrije Universiteit Amsterdam:
<ul>
    <li> [MSc research project] Duc Anh Phan — <i> LLM KV Cache Performance Characterization When Using Disk Offloading for Prefix Caching </i> - <a href="{{ site.url }}/downloads/supervised_isp_phan_llm.pdf" style="color:#009988">PDF</a> <a href="https://github.com/anhphantq/kv-cache-offloading-benchmarking" style="color:#009988">Code</a> - 2025 </li>
    <li> [MSc thesis] Joseph Kanichai — <i>Characterizing The Energy Contribution and Energy-Performance Trade-offs of NVMe SSDs in the Linux Storage Stack</i> — <a href="{{ site.url }}/downloads/supervised_thesis_joseph_kanichai_ssd_energy.pdf" style="color:#009988">PDF</a> <a href="https://github.com/t348575/energy-benchmark" style="color:#009988">Code</a> — 2025 </li>
    <li> [BSc thesis] Yigit Abaci — <i>A Performance Analysis of TC for High Speed, Scalable Data Center Networks </i> — <a href="{{ site.url }}/downloads/supervised_thesis_yigit_abaci_tc.pdf" style="color:#009988">PDF</a> — 2025 </li>
    <li> [BSc HP project] Gleb Mischenko — <i>PokeSto: A Storage Benchmark for Modifiable Virtual Environments</i> — <a href="{{ site.url }}/downloads/supervised_hp_gleb_mischenko_mve.pdf" style="color:#009988">PDF</a> <a href="https://github.com/atlarge-research/yardstick" style="color:#009988">Code</a> - 2025 </li>
    <li> [MSc thesis] <a href="https://medium.com/@appsby12">Sudarsan Sivakumar</a> — <i>Performance Characterization Study of NVMe Storage Over TCP</i> — <a href="{{ site.url }}/downloads/supervised_thesis_sudarsan_sivakumar_NVMeoFTCP.pdf" style="color:#009988">PDF</a> <a href="https://github.com/stonet-research/NVMeoFTCP-Characterization" style="color:#009988">Code</a> — 2024 </li>
    <li> [BSc thesis] Darko Vujica — <i>Exploring Redis Persistence Modes: Introducing AOFURing, an io_uring AOF Extension</i> —  <a href="{{ site.url }}/downloads/supervised_thesis_darko_vujica_aofuring.pdf" style="color:#009988">PDF</a> <a href="https://github.com/daraccrafter/Thesis-Redis-IO_Uring" style="color:#009988">Code</a> — 2024 </li>
    <li> [BSc thesis] Vincent Kohm — <i>Optimizing Metadata Handling with vkFS: A Hybrid Key-Value Store File System leveraging RocksDB</i> — <a href="{{ site.url }}/downloads/supervised_thesis_vincent_kohm_vkfs.pdf" style="color:#009988">PDF</a> <a href="https://github.com/Vincent881909/vkfs" style="color:#009988">Code</a> — 2024 </li>
    <li> [MSc survey] <a href="https://medium.com/@appsby12">Sudarsan Sivakumar</a> — <i>A survey on flash storage disaggregation: performance and quality of service considerations</i> — <a href="{{ site.url }}/downloads/supervised_survey_sudarsan_sivakumar_flash_storage_disaggregation_qos.pdf" style="color:#009988">PDF</a> —  2024 </li>
</ul>

<h2> University Courses </h2>

For my PhD at Vrije Universiteit Amsterdam, I was involved as a teaching assistant with coordinating roles for the following courses:
<ul>
    <li> [2023–2025] — <a href="https://research.vu.nl/en/courses/systems-seminar"> System Seminar (MSc)</a>: Teaching students how to read <i>and</i> review systems papers. Topics changed yearly and we have covered topics ranging from storage, networks, accelerators, programming language runtimes, data center carbon footprint, security, to LEO sattelites. Additionally, in 2023-2024, students were given the opportunity to reproduce systems artifacts and write a system artifact review. I was responsible for the lab practicals and managing the system artifacts. Lastly, I was involved in grading the reviews and work distribution for the TAs. </li>
    <li> [2025] — <a href="https://atlarge-research.com/courses/advanced-net-prog-vu"> Advanced Systems Programming (BSc)</a>: The spirital successor of the "Advanced Network Programming'' course. Now teaching students how to design, implement, and evaluate broader systems software. The lab projects in 2025 focused on the NodeJS runtime and on implementing a HTTPS stack in NodeJS through C (cross-language complexities). I was a supporting TA for this course (advising my succeeding lead TA) and a webmaster.</li>
    <li> [2023–2024] — <a href="https://atlarge-research.com/courses/advanced-net-prog-vu"> Advanced Network Programming (BSc, discontinued)</a>: Teaching students how to design, implement, and evaluate network stacks. Students had to implement ICMP and TCP in user-space for Linux using C. I was lead TA for this course, leading the other TAs. I had coordination, grading, interviewer, lab practical, and contact person roles.</li>
    <li> [2024] — <a href="https://atlarge-research.com/courses/distr-sys-vu/"> Distributed Systems (MSc)</a>: Teaching students how to design, implement, and evaluate distributed systems. Students can pick a project that aligns with their interest; I gave storage systems related projects to several groups.</li>
        <ul>
            <li> Dissagregated RocksDB (2024): Teaching students about dissagregated storage, I/O interfaces, RocksDB, and performance. In this project, students modify RocksDB to allow swapping the I/O interface through a file system plugin, and evaluate the performance impact of I/O interfaces on local and dissagregated storage. See
            <a href="{{ site.url }}/downloads/bose-et-al-2024.pdf" style="color:#009988">bose-et-al.pdf</a> and
            <a href="{{ site.url }}/downloads/anh-et-al-2024.pdf" style="color:#009988">anh-et-al.pdf</a>.
            </li>
        </ul>
     <li> [2023] — <a href="https://atlarge-research.com/courses/storage-systems-vu/"> Storage Systems (MSc, discontinued)</a>: StoNet's flagship course. Here we taught students how to design, implement and evaluate storage systems. Students had to implement an FTL, a GC algorithm, and an FS for the NVMe ZNS interface. I was a lead TA (along with Matthijs Jansen) and I had roles related to coordination, grading, interviewing students, maintaining the grading/competition framework, server provisioning, lab practicals, and student contact person. I also provided educational material for KV-stores. We published our efforts in <a href="https://ieeexplore.ieee.org/abstract/document/10701387">CCGRID'24</a></li>
</ul>

<h2> Academic service </h2>

I have reviewed conference papers from HPDC'23, CCGRID'24, ICPE'24, Middleware'25, and ACM TOS'25 (and given advice on USENIX ATC'24 reviews). I have also reviewed system artifacts from SOSP'23.
