# TASK 10 – Measure and Compare

## Introduction
System performance can be evaluated by measuring execution time, system calls and resource usage.

## Commands Used

1. Compile the file-copy program:

gcc -std=c11 -Wall -Wextra copy.c -o copy

2. Measure system calls:

strace -c ./copy

3. Measure resource usage:

/usr/bin/time -v ./copy

4. Measure process execution:

time ./process

5. Measure 1000 process creations:

time bash -c 'for i in $(seq 1 1000); do /bin/true; done'

## Process vs Thread Comparison

Processes have separate memory spaces and provide better isolation.

Threads share the same memory space and are generally lighter to create.

## Observations

- Larger buffers reduce read() calls.
- Threads generally require fewer resources than separate processes.
- Processes provide better memory isolation.
- Execution time depends on CPU load and system configuration.

## Conclusion
Performance measurement helps identify efficient ways to manage processes, threads and system calls.