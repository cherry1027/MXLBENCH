# MXLBench

A two-page React/TypeScript prototype for modeling high-bandwidth media workloads and exploring benchmark measurements.

## Live demo

https://mxlbench-lab.charanvaranasi44.workers.dev

## Features

- Configurable producer–consumer topology
- Stream count, resolution, frame rate, and CPU controls
- Automatic raw-data-rate calculations
- Clearly labeled simulated bottlenecks
- Benchmark explorer with simulated reference runs
- CSV import for actual measurements
- MXL vs shared-memory comparison
- Responsive interface

> MXLBench is a UI prototype. It has no backend, performs no real MXL integration, and does not claim measured MXL performance.

## CSV format

Import a CSV with these columns:

```csv
id,transport,topology,resolution,fps,streams,cpu_cores,throughput_gbps,latency_ms,dropped_frames
RUN-001,MXL,4P → 2C,4K,60,6,8,115.2,4.8,0
RUN-002,Shared memory,4P → 2C,4K,60,6,8,101.7,6.1,12
