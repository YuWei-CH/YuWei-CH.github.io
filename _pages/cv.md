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
* B.S. in Computer Science, New York University, 2021 - 2025 (expected)

Work experience
======
* Fall 2024 - Present: Research Intern
  * **Improved a wafer-scale GPU simulator** using the Akita engine and MGPUSim framework, investigating the impact of various memory structures on kernel time, throughput, cache hit/miss rate, and CPI.
  * Optimized the data communication by implementing a local address-only TLB and separate page tables for GMMU across multiple GPUs.
  * Supervisor: Professor Yifan Sun

* Spring 2024 - Present: Undergraduate Researcher
  * **Translated CUDA source code to HIP** using HIPify tools, enabling AMD GPU support and achieving out-of-the-box GPU acceleration for AlphaFold and DualPhysics with OverlayFS and Singularity.
  * **Contributed to the open-source HIPify repository** by identifying and resolving Math_constant.h missing, enhancing CUDA-to-HIP translation for broader compatibility within ROCm platform.
  * Participated in ARM migration on Graviton CPUs in Amazon Web Services (AWS) and Axion CPUs in Google Cloud Platform (GCP), compiling HPL, Amber24, and Gaussian to evaluate ARM CPU suitability. Calculated price-performance metrics and documented compatible libraries and compiler optimization flags.

* Summer 2024: HPC Assistant
  * Enhanced [Reform](https://github.com/gencorefacility/reform), a genome sequence editing tool, by adding **sequential processing, compressed file handling, and parallel execution**.
  * Updated [ReformWeb](https://reform.bio.nyu.edu/), enabling users to run Reform on HPC servers via a Web UI. Integrated new Reform features and verbose email notification using Flask, SQLite, Redis, Werkzeug, and Jinja2. Created dev and cached test sites.
  * Established a CI/CD pipeline with GitHub Actions and Python unittest, cutting build and test time to enhance development efficiency. Designed a Bash-based pipeline for verification, applying a 7-day TTL for successful results and retaining logs and failed uploads for debugging.

<!-- Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul> -->

Projects
======
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
* Technicals: Git/Github, Linux, OpenMP, MPI, GCP, CI/CD, Raspberry Pi;