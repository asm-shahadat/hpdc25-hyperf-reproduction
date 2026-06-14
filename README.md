# Reproducing ACM HPDC '25: HYPERF

This repository contains a Chameleon Trovi reproduction artifact for the ACM HPDC '25 paper:

**HYPERF: End-to-End Autotuning Framework for High-Performance Computing**

## Overview

HYPERF is an end-to-end autotuning framework for improving the performance of high-performance computing benchmark programs. The original paper evaluates HYPERF on a larger set of PolyBench and Rodinia benchmarks using a full autotuning campaign.

This artifact reproduces a scaled subset of the paper's evaluation for Chameleon Trovi. The goal is to reproduce the main benchmark-evaluation workflow using selected PolyBench/Rodinia programs and input sizes.

## Reproduction Scope

This artifact focuses on:

1. A scaled Figure 10-style Rodinia normalized-runtime comparison.
2. A scaled Figure 7-style PolyBench subset normalized-runtime comparison.
3. Optional autotuning-progress or optimization-overhead results.


## Platform

The intended platform is:

* Chameleon Trovi
* CHI@UC bare-metal CPU node
* Ubuntu 22.04
* CPU/OpenMP benchmark execution

## Expected Outputs

The artifact generates result files in:

```text
results/
```

and reproduced figures in:

```text
figures/
```

Expected figures include normalized-runtime plots comparing baseline benchmark execution with optimized or autotuned variants.

## Notes

This artifact uses actual benchmark programs and input sizes where possible, but scales down the number of benchmarks and tuning iterations for reproducibility and replayability. Absolute runtime values are not expected to exactly match the paper because the hardware, system load, and tuning budget may differ from the original evaluation.
