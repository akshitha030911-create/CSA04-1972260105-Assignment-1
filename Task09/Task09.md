# TASK 09 – Memory Hierarchy and I/O

## Introduction
Memory hierarchy organizes storage according to speed, capacity and cost.

## Types of Memory

1. Registers and Cache:
Very fast memory used by the CPU for active calculations.

2. RAM:
Temporary memory used for running programs and storing active data.

3. SSD:
Provides fast and permanent storage.

4. Hard Disk and Network Storage:
Used for large data storage, backups and archives.

## Applications in Smart Hospitals

- Patient-monitor readings are temporarily stored in RAM.
- Patient records are stored in reliable database storage.
- MRI images are processed using RAM and SSD storage.
- Long-term medical images are stored in archives.

## Types of I/O

1. Programmed I/O:
The CPU repeatedly checks device status.

2. Interrupt-Driven I/O:
The device sends an interrupt when it requires attention.

3. Direct Memory Access (DMA):
Transfers data directly between a device and memory with less CPU involvement.

## Recommended Method

DMA is suitable for MRI image transfers because it handles large amounts of data efficiently.

## Comparison

Programmed I/O requires continuous CPU attention.

Interrupt-driven I/O reduces unnecessary checking.

DMA provides efficient block transfers and reduces CPU workload.

## Conclusion
Proper memory management and DMA improve the performance of hospital systems, especially MRI imaging servers.