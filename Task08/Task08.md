# TASK 08 – CPU States and Protection

## Introduction
The CPU operates in two main modes: user mode and kernel mode.

## 1. User Mode
- Used by application programs.
- Has limited access to hardware.
- Cannot execute privileged instructions.

## 2. Kernel Mode
- Used by the operating-system kernel.
- Has complete access to hardware.
- Can execute privileged instructions.

## Mode Switching
A system call or exception transfers control from user mode to kernel mode.

A hardware interrupt also transfers control to the operating system.

## Timer Interrupt
A timer interrupt allows the operating system to regain CPU control and schedule other processes.

## Memory Protection
Memory Management Unit (MMU) protects memory by preventing unauthorized access between processes.

## Importance in Smart Hospitals
If a patient-monitoring application could disable interrupts, the operating system might fail to respond to important sensor events.

Therefore, hardware protection and interrupt handling are essential.

## Polling vs Interrupts

Polling repeatedly checks whether a device needs attention.

Interrupt-driven I/O allows the device to notify the CPU when an event occurs.

Interrupt-driven processing is more suitable for patient monitoring because it reduces unnecessary CPU activity.

## Conclusion
CPU protection mechanisms ensure security, stability and reliable operation in smart hospitals.