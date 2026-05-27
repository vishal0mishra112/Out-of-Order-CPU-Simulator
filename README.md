# Out-of-Order (OoO) CPU Performance Simulator

> 🚧 **Status:** Active Development & Architectural Planning

## 📌 Project Overview
This repository hosts the development of a cycle-accurate software simulator designed to model Out-of-Order (OoO) instruction execution, latency, and Instructions Per Cycle (IPC) for high-performance, server-class workloads. 

As modern CPU architectures rely heavily on deep pipelines and complex memory hierarchies, identifying execution bottlenecks is critical. This simulator leverages both C++ and SystemVerilog to model the microarchitecture and uses data-driven techniques to profile pipeline efficiency, branch prediction accuracy, and cache throughput.

## 🚀 Key Features (In Development)
* **Cycle-Accurate Modeling:** Core execution engine built in `C++` to accurately simulate clock cycles, instruction fetching, decoding, and OoO execution using data structures like Reorder Buffers (ROB) and Reservation Stations.
* **Pipeline Bottleneck Tracking:** Advanced logging to track and analyze pipeline stalls, structural hazards, and data dependencies.
* **Branch Prediction Profiling:** Implementation of branch prediction algorithms to measure misprediction penalties and efficiency.
* **Cache Memory Subsystem:** Simulating memory hierarchy throughput, cache hits/misses, and memory access latency.
* **Hardware/Software Integration:** Interfacing with `SystemVerilog` for hardware-level RTL verification and correlation of specific architectural blocks.

## 🛠️ Tech Stack
* **Core Simulator:** C++
* **Hardware Description & RTL:** SystemVerilog
* **Data Analytics & Profiling:** Python (Pandas/Matplotlib for log analysis)
* **Build System:** Linux / Make

## 🗺️ Development Roadmap
- [x] **Phase 1:** Repository initialization and definition of the basic instruction set architecture (ISA) subset.
- [ ] **Phase 2:** Develop the in-order instruction fetch and decode pipeline stages in C++.
- [ ] **Phase 3:** Implement Out-of-Order execution logic (issue, execute, write-back) and data hazard resolution.
- [ ] **Phase 4:** Integrate the branch prediction module and hierarchical cache memory model.
- [ ] **Phase 5:** SystemVerilog integration for specific module verification and correlation.
- [ ] **Phase 6:** Extensive benchmarking, bottleneck analysis, and documentation.

## 👨‍💻 Author
**Vishal Kumar Mishra**
* [LinkedIn](https://linkedin.com/in/VishalMishra)
* [GitHub](https://github.com/VishalMishra112)

---
*Note: This is an ongoing project. Core engine code and hardware modules will be pushed incrementally in phases over the upcoming weeks.*
