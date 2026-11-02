# TASK 06 – Cost of System Calls

## Introduction
System calls require switching between user mode and kernel mode. Therefore, they are more expensive than ordinary function calls.

## Effect of Buffer Size

For a 10,000-byte file:

- 1-byte buffer: 10,001 read() calls.
- 512-byte buffer: 21 read() calls.
- 4096-byte buffer: 4 read() calls.

Larger buffers reduce the number of system calls and improve performance.

## C Program

The following program copies a file using different buffer sizes and counts read() calls.

## Conclusion
Using larger buffers reduces system-call overhead and improves file-copying efficiency.