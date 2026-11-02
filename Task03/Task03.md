# TASK 03 – Operating-System Structures

## Types of Operating-System Structures

1. Monolithic Structure
All major operating-system services run inside the kernel.
Advantage: Fast performance.
Disadvantage: A faulty component can affect the entire system.

2. Layered Structure
The operating system is divided into different layers.
Advantage: Easy to maintain.
Disadvantage: Communication between layers may cause overhead.

3. Microkernel Structure
Only essential services run inside the kernel.
Advantage: Better security and fault isolation.
Disadvantage: Communication between services may increase overhead.

4. Modular Structure
The kernel supports dynamically loadable modules.
Advantage: Flexible and efficient.
Disadvantage: Faulty modules can affect the kernel.

5. Hybrid Structure
Combines features of monolithic and microkernel structures.
Advantage: Balances performance and flexibility.
Disadvantage: Complex implementation.

## Recommended Structures

For patient monitors, a microkernel-based real-time operating system such as QNX is suitable because it provides fault isolation.

For database servers, Linux is suitable because it supports modular architecture, security and clustering.

## Examples
- Linux – Monolithic but modular.
- Windows – Hybrid.
- Android – Based on Linux kernel.
- QNX – Microkernel.
- FreeRTOS – Real-time kernel.

## Conclusion
Microkernel-based systems are suitable for critical monitoring devices, while modular server operating systems are suitable for hospital databases.