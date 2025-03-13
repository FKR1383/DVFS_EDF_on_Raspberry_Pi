# Embedded Systems Project: Dynamic Voltage and Frequency Scaling (DVFS) on Raspberry Pi

## Overview
This project focuses on optimizing power consumption in a multi-core embedded system, specifically a Raspberry Pi, using Dynamic Voltage and Frequency Scaling (DVFS). The goal is to manage power consumption dynamically by adjusting the CPU frequency based on task deadlines and workload. We implemented a scheduling algorithm that combines Earliest Deadline First (EDF) with DVFS to minimize energy consumption while meeting task deadlines.

## Key Features
- **DVFS Implementation**: Dynamically adjusts CPU frequency to optimize power consumption.
- **EDF Scheduling**: Ensures tasks are executed in order of their deadlines.
- **Power Profiling**: Measures power consumption of benchmark tasks using a USB Power Meter.
- **Benchmarking**: Utilizes the MiBench benchmark suite to evaluate performance and power consumption.

## Project Steps
1. **Setup Raspberry Pi**: Configure the Raspberry Pi with Raspberry Pi OS.
2. **Run Benchmark Tasks**: Execute tasks from the MiBench benchmark suite.
3. **Frequency Range Analysis**: Determine the allowable frequency range for each CPU core.
4. **Power Profiling**: Measure execution time and power consumption for benchmark tasks at different frequency levels.
5. **Scheduling Algorithm**: Implement an EDF-based scheduler with DVFS to optimize task execution and power usage.
6. **Simulation**: Simulate task execution on Raspberry Pi cores using the scheduling algorithm.
7. **Results Analysis**: Compare power consumption with and without DVFS.

## Tools and Technologies
- **Raspberry Pi**: Used as the target embedded system.
- **MiBench**: Benchmark suite for evaluating performance.
- **USB Power Meter**: Hardware tool for measuring power consumption.
- **Bash Scripts**: Automated task execution and power profiling.

## Results
The project successfully demonstrated that using DVFS in combination with EDF scheduling can significantly reduce power consumption while maintaining task deadlines. The implemented algorithm showed good performance, with most tasks meeting their deadlines and power consumption being minimized.

## Future Improvements
- **Slack Time Distribution**: Distribute remaining time among tasks to further optimize deadlines.
- **Thread Utilization**: Use threads to reduce computational overhead in the offline scheduling phase.

## Conclusion
This project highlights the importance of power management in embedded systems and demonstrates how DVFS can be effectively used to optimize energy consumption while meeting real-time task deadlines. The results show that the implemented scheduling algorithm is a viable solution for power-efficient embedded systems.

For more details, refer to the full project documentation and code in the repository.
