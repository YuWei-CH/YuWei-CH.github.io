---
layout: archive
# title: "Yuwei Sun's CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.S. in Computer Science, New York University, 2021 - 2025 (University Honors)
* Master of Computer Science, University of Illinois Urbana-Champaign, 2025 - 2027 (expected)

Work experience
======

* Summer 2025: High Performance Computing Intern
  * Extended [nifty-ls](https://github.com/flatironinstitute/nifty-ls), a Lomb-Scargle periodogram tool, to support multiple sinusoidal basis terms, improving model flexibility and enabling detection of complex periodic patterns in irregular time-series data.
  * Identified performance bottlenecks via cProfile and achieved a 100× speedup by offloading and parallelizing compute-heavy routines from Python to C++ with nanobind and OpenMP.
  * Resolved GPU out-of-memory issues by distributing batched computation across multiple GPUs using CuPy, enabling large-scale, memory-bound workloads and improving scalability by additional 50×.
  * Reduced the 99th-percentile numerical error of the FastChi2 method from 1e-3 to 1e-6 by rewriting thetrigonometric summation and replacing NumPy FFT with FINUFFT for improved numerical precision.

* Fall 2024 - Spring 2025: Part-time Research Engineer
  * Benchmarked and compiled Gaussian and Amber on ARM CPU–based NVIDIA Grace Hopper nodes, evaluating energy efficiency, performance, and software compatibility of ARM CPUs.
  * Led the migration from a physical HPC cluster to an on-premises cloud based on OpenShift, developing a pipeline that synchronized the cluster environment to   OpenShift using Podman, Singularity, and Kubernetes.

* Fall 2024 - Spring 2025: Research Intern
  * **Improved a wafer-scale GPU simulator** using the Akita engine and MGPUSim framework, investigating the impact of various memory structures on kernel time, throughput, cache hit/miss rate, and CPI.
  * Optimized the data communication by implementing a local address-only TLB and separate page tables for GMMU across multiple GPUs.
  * Supervisor: Professor Yifan Sun

* Summer 2024: HPC Assistant
  * Enhanced [Reform](https://github.com/gencorefacility/reform), a genome sequence editing tool, by adding **sequential processing, compressed file handling, and parallel execution**.
  * Updated [ReformWeb](https://reform.bio.nyu.edu/), enabling users to run Reform on HPC servers via a Web UI. Integrated new Reform features and verbose email notification using Flask, SQLite, Redis, Werkzeug, and Jinja2. Created dev and cached test sites.
  * Established a CI/CD pipeline with GitHub Actions and Python unittest, cutting build and test time to enhance development efficiency. Designed a Bash-based pipeline for verification, applying a 7-day TTL for successful results and retaining logs and failed uploads for debugging.

* Spring 2024: Part-time Research Engineer
  * **Translated CUDA source code to HIP** using HIPify tools, enabling AMD GPU support and achieving out-of-the-box GPU acceleration for AlphaFold and DualPhysics with OverlayFS and Singularity.
  * **Contributed to the open-source HIPify repository** by identifying and resolving Math_constant.h missing, enhancing CUDA-to-HIP translation for broader compatibility within ROCm platform.
  * Participated in ARM migration on Graviton CPUs in Amazon Web Services (AWS) and Axion CPUs in Google Cloud Platform (GCP), compiling HPL, Amber24, and Gaussian to evaluate ARM CPU suitability. Calculated price-performance metrics and documented compatible libraries and compiler optimization flags.

Publications
======
<ul>
  <li>
    Our work 
    <a href="https://ieeexplore.ieee.org/abstract/document/11096405" target="_blank">
      Luthier: A Dynamic Binary Instrumentation Framework Targeting AMD GPUs
    </a> 
    has been accepted to <strong>ISPASS 2025</strong>! I am a co-author.
  </li>
</ul>

<!-- 
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul> 
-->

Projects
======
* Travel Planner (AWS-Sponsored)
  * Secured AWS technical sponsorship and cloud credits by pitching the project to a team of Solutions Architects.
  * Led the development of a serverless, auto-scaling travel planner on AWS (Lambda, RDS, Cognito, API Gateway), integrating LLM-based trip recommendations and OCR-based ticket parsing.
  * Implemented an event-driven architecture with SQS and reduced OpenAI APl cost by ~30% using ElastiCache.

* Google Hardware Product Sprint (HPS) Participant - EE Track
  * Designed, tested, and fabricated a [PCB-based clock](https://github.com/YuWei-CH/RedSun_Clock) through KiCAD using microcontrollers(atmega328), LED Matrix, Crystal Clock and programming by C.

* Byte-Pi-Cluster
  * Built [Byte-Pi-Cluster](https://github.com/YuWei-CH/Byte-Pi-Cluster) with a 5-nodes Raspberry Pi cluster integrating Kubernetes and MPI, and NFS for shared storage, enabling secure public network access via FRP.

Fellowship
======
* Uber Career Prep: SDE Fellowship (4% acceptance rate)
  * Completed 6 months of software engineering training and 14 coaching sessions with senior engineers and product managers.
  * Mastered inclusive design, documentation, and teamwork by working with a product manager to develop a Product Requirements Document for a scenario in providing Uber rides to underage riders in San Francisco.

Compeition
======
* Student Cluster Competition (6th place globally)
  * **Optimized HPC benchmarks performance** using Intel oneAPI, Nvidia HPC SDK, and targeted compile flags on Intel MAX 9480 CPUs (with High Bandwidth Memory) and Nvidia A100 GPUs.
  * Strategized application runtime and CPU cores usage to reduce energy consumption and improve CPU utilization.

Skills
======
* Languages: Python, C/C++, SQL, CUDA;
* Framework: Flask, Redis, MySQL, Docker, SLURM, Singularity, CMake;
* Technicals: Git/Github, Linux, OpenMP, MPI, GCP, CI/CD, Raspberry Pi, cProfile;