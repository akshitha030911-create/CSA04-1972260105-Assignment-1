# TASK 05 – System Calls

## Introduction
System calls provide an interface between user programs and the operating-system kernel.

## Types of System Calls

1. Process Control:
fork(), exec(), wait(), exit().

2. File Management:
open(), read(), write(), close().

3. Device Management:
Requesting and controlling hardware devices.

4. Information Maintenance:
Getting system information and process details.

5. Communication:
Pipes and sockets.

6. Protection:
Managing permissions and access control.

## Working of read() System Call

1. A program calls the read() function.
2. The system-call number and arguments are passed to the kernel interface.
3. The CPU switches from user mode to kernel mode.
4. The kernel validates the file descriptor and arguments.
5. The kernel performs the requested input operation.
6. The result is returned to the user program.

## System Call Monitoring

The strace command is used to observe system calls.

Example:

strace -e trace=openat,read,write,close ./program

## Alternative

C library functions such as fopen(), fread() and fwrite() provide buffered file operations.

Buffering reduces the number of system calls and improves performance.

## Conclusion
System calls allow applications to access operating-system services safely and efficiently.