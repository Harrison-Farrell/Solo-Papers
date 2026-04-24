# Solo Papers

A collection of technical papers, case studies, and articles authored by Harrison T. Farrell, focusing on low-level performance optimization, hardware-aware software design, and C++ data structures.

## Papers

### [Analysis of CPU-Level Optimizations in Graph-Based Search: A Boggle Solver Case Study](./boggle.pdf)
**Date:** April 22, 2026

This paper investigates the impact of hardware-aware software design on the performance of a graph-based search problem (Boggle). By transitioning from a standard high-level implementation to a hardware-optimized model, an 11.0× throughput increase was achieved. The case study analyzes the efficacy of:
- Mitigating the "Memory Wall" through arena allocation
- Reducing branch misprediction penalties via bitmasking
- Leveraging hardware-accelerated bitwise instructions (e.g., BMI1/BMI2)

The findings suggest that performance in modern CPUs is heavily dependent on memory-subsystem and execution-pipeline harmony rather than algorithmic complexity alone.

### [CPU Cache and the Impact to Data Structures](./cpu_cache.pdf)
**Date:** February 18, 2026

This article explores how CPU cache impacts the performance of both contiguous and non-contiguous data structures. It compares four common data structures from the C++ Standard Library (unsorted vector, sorted vector, set, and unordered set). The analysis demonstrates that while search algorithms may share the same Big O time complexity, their real-world performance can differ significantly due to CPU architecture, particularly cache latency and hardware pre-fetching behaviors.
