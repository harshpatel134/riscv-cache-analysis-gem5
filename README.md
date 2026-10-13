# Analysis of Cache Size and Associativity in RISC-V Using GEM5

## Overview

This project analyzes the effect of L1 data cache size and associativity on RISC-V processor performance using the GEM5 architectural simulator.

Two experiments were conducted by varying cache size and associativity independently while keeping other system parameters constant.

## Objectives

- Analyze the effect of L1 data cache size on cache performance.
- Study the impact of cache associativity on hit rate and miss rate.
- Evaluate processor performance using Cycles Per Instruction (CPI).
- Understand the relationship between cache configuration and processor performance.

## Simulation Environment

- Simulator: GEM5 23.0.0.1
- Architecture: RISC-V
- CPU Model: RiscvTimingSimpleCPU
- Clock Frequency: 1 GHz
- Simulation Mode: System-call Emulation (SE)
- Programming Language: C (workloads), Python (GEM5 configuration)

## Experiments

### 1. L1 Data Cache Size Analysis

The cache size was varied while keeping associativity fixed at 4-way.

Tested configurations:
- 8 KB
- 16 KB
- 32 KB
- 64 KB

### 2. L1 Data Cache Associativity Analysis

Associativity was varied while keeping cache size fixed at 16 KB.

Tested configurations:
- 2-way
- 4-way
- 8-way
- 16-way

## Results

### Cache Size Experiment

Increasing L1 data cache size from 8 KB to 64 KB improved the hit rate from 92.08% to 99.98% and reduced CPI by approximately 15%.

### Cache Associativity Experiment

Increasing associativity from 2-way to 16-way improved the hit rate from 95.65% to 99.41% and reduced CPI by approximately 8.76%.

## Performance Metrics

- Cache Hit Rate
- Cache Miss Rate
- CPU Cycles
- Instructions
- Cycles Per Instruction (CPI)

## Tools Used

- GEM5
- RISC-V
- Python

## Project Report

[View the detailed project report](RISC-V_Cache_Analysis_Report.pdf)

## Conclusion

The simulation results demonstrate how increasing cache size and associativity can improve L1 data cache performance and reduce processor execution overhead for the workloads used in this study.
