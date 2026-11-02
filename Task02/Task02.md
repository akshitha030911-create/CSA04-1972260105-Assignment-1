# TASK 02 – Types of Operating Systems

## 1. Introduction

A smart hospital requires different types of operating systems based on the requirements of each computing environment.

## 2. Recommended Operating Systems

| Environment | Recommended OS | Reason |
|---|---|---|
| Patient Monitors | Hard Real-Time OS | Provides predictable response within strict deadlines. |
| Nurses' Tablets | Mobile OS | Supports battery management and wireless communication. |
| Doctors' Workstations | Desktop OS | Supports multitasking and medical applications. |
| Patient Database | Clustered Server OS | Provides high availability and data recovery. |
| MRI Imaging Server | Multiprocessor OS | Supports parallel processing and high throughput. |
| Partner Hospitals | Distributed OS Environment | Supports communication and data sharing between hospitals. |

## 3. Hard Real-Time vs Soft Real-Time

**Hard Real-Time OS:**
- Must complete critical tasks within fixed deadlines.
- Missing a deadline can cause serious consequences.
- Suitable for patient monitoring and alarm systems.

**Soft Real-Time OS:**
- Tries to complete tasks within deadlines.
- Occasional delays may be acceptable.
- Suitable for non-critical multimedia and general applications.

## 4. Symmetric vs Asymmetric Multiprocessing

**Symmetric Multiprocessing (SMP):**
- Multiple processors share memory.
- All processors can execute operating-system tasks.
- Provides efficient parallel processing.
- Suitable for MRI image processing.

**Asymmetric Multiprocessing (AMP):**
- Different processors are assigned specific tasks.
- One processor may control or coordinate other processors.
- Useful in specialised embedded systems.

## 5. Why a Clustered Server OS?

A clustered server uses multiple connected computers to provide services.

Advantages:
- High availability.
- Fault tolerance.
- Load balancing.
- Data replication.
- Better reliability.

If one server fails, another server can continue providing services.

## 6. Why a Distributed System?

A distributed system allows multiple computers to communicate and share resources.

It is useful for connecting the main hospital with partner hospitals.

Advantages:
- Secure information sharing.
- Resource sharing.
- Scalability.
- Improved availability.

## 7. Performance and Complexity

- SMP improves parallel processing performance.
- Clustering reduces dependence on a single server.
- Distributed systems improve resource sharing.
- Real-time operating systems provide predictable response times.

However, these systems require additional hardware, maintenance and administration.

## 8. Conclusion

Different operating-system types are required for different hospital environments. A combination of real-time, mobile, desktop, clustered server and distributed systems provides better performance, security and reliability for a smart hospital.