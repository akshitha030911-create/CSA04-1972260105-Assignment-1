# TASK 07 – Process Control System Calls

## Introduction
Process control system calls are used to create, execute and terminate processes.

## Important System Calls

1. fork() – Creates a new child process.
2. exec() – Replaces the current process with another program.
3. wait() – Waits for a child process to finish.
4. exit() – Terminates a process.
5. waitpid() – Waits for a specific child process.

## Zombie Process
A zombie process is a process that has finished execution but whose exit status has not yet been collected by its parent.

## Orphan Process
An orphan process is a running process whose parent has terminated.

## Working
A shell creates a child using fork(). The child executes a command using exec(). The parent waits using wait() and collects the exit status.

## Conclusion
Process control system calls help the operating system manage multiple processes efficiently.