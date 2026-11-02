# TASK 01 – Requirements of Each Computing Environment

## 1. Introduction

A smart hospital requires different operating systems for different computing environments. Each system has different requirements for response time, reliability, throughput, battery efficiency and security.

## 2. Ranked Requirement Analysis

| Environment | Priority 1 | Priority 2 | Priority 3 |
|---|---|---|---|
| Patient Monitors | Response time | Reliability | Security |
| Nurses' Tablets | Battery life | Security | Response time |
| Doctors' Workstations | Performance | Security | Reliability |
| Database Server | Reliability | Security | Throughput |
| Imaging Server | Throughput | Performance | Reliability |
| Partner Hospitals | Security | Reliability | Data sharing |

### Justification

1. Patient Monitors:
Must detect abnormal readings and generate alarms within 10 milliseconds. Response time and reliability are critical for patient safety.

2. Nurses' Tablets:
Must operate throughout a complete work shift. Battery efficiency and secure access to patient information are important.

3. Doctors' Workstations:
Must provide fast access to medical records, reports and hospital applications. Performance and security are essential.

4. Database Server:
Must continuously store and retrieve patient records. Reliability and data protection are the highest priorities.

5. Imaging Server:
Must process large MRI images using multiple processors. High throughput and processing performance are required.

6. Partner Hospitals:
Must securely exchange patient information. Network reliability, authentication and data security are essential.

## 3. Conflicting Requirements

Some requirements conflict with each other:

- Fast response time may conflict with heavy processing workloads.
- High throughput may increase resource usage.
- Strong security checks may introduce processing overhead.
- Battery saving may reduce processor performance.
- Continuous availability requires additional hardware and maintenance.

Therefore, one general-purpose operating system may not satisfy every hospital requirement equally.

## 4. Patient Safety Requirements

Patient monitors and the central database are the most critical systems.

- Patient monitors must generate alarms within 10 milliseconds.
- The database must prevent loss of patient records.
- Reliable communication must be maintained between medical devices and servers.
- Security must prevent unauthorized access to confidential medical information.

A delay or failure in these systems may affect patient care.

## 5. Lessons from the History of Operating Systems

- Batch Systems: Useful for processing large amounts of hospital billing and administrative data.
- Time-Sharing Systems: Allow multiple doctors and nurses to access shared computing resources.
- Personal Computer Systems: Support doctors' desktop applications.
- Mobile Operating Systems: Support portable nursing tablets with battery management and wireless connectivity.

Modern operating systems combine these developments to support different hospital environments.

## 6. Alternative Concept: One General-Purpose OS Everywhere

If the hospital uses one general-purpose operating system on every device, administration may become simpler.

However, it has several disadvantages:

1. Alarm Response:
A general-purpose OS cannot guarantee a strict 10 ms deadline because other processes may delay execution. A real-time OS can provide bounded and predictable response times.

2. Memory:
A general-purpose OS may require more memory and processing resources than a lightweight embedded OS, making it unsuitable for small patient monitors.

3. Administration:
Using one OS simplifies updates and maintenance, but it cannot provide the specialized performance and reliability required by every device.

## 7. Final Evaluation

A single general-purpose operating system is not suitable for the entire smart hospital.

A real-time OS should be used for patient monitors, mobile OS for nurses' tablets, desktop OS for doctors' workstations, clustered server systems for patient records and multiprocessor systems for MRI processing.

This mixed operating-system approach provides better safety, reliability, performance and scalability.