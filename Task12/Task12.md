# TASK 12 – Day-4 Design Challenge

## Introduction
The smart hospital is expanding its services by introducing home patient monitoring and cloud-based medical records.

The original operating-system design must be modified to support these new requirements.

## A. Impact Analysis

Home monitoring introduces:
- Internet connectivity.
- Remote patient monitoring.
- Device authentication.
- Secure data transmission.
- Remote software updates.

Cloud-based records introduce:
- Data sharing.
- Large-scale storage.
- Data security.
- Backup and recovery.
- High availability.

## B. Evaluation of Original Design

The original design is still suitable for bedside patient monitors because local real-time processing can provide fast alarm responses.

However, home monitoring devices require additional communication and security features.

Cloud-based medical records improve accessibility and scalability but require strong protection mechanisms.

## C. Adapted Operating-System Plan

1. Home Monitoring Devices:
Use embedded real-time operating systems.

2. Cloud Medical Records:
Use distributed cloud-based services with replicated storage.

3. Data Communication:
Use encrypted communication and authentication.

4. Data Backup:
Maintain regular backups and recovery mechanisms.

5. Local Alarm Processing:
Critical alarms must be processed locally without depending entirely on internet connectivity.

6. Remote Updates:
Use authenticated and secure software updates.

## D. Justification

The original design should be modified rather than completely replaced.

The existing operating systems are suitable for their respective environments. Additional cloud services, security mechanisms and communication systems can support the new requirements.

## Advantages

- Improved remote patient monitoring.
- Secure medical record sharing.
- Better data availability.
- Increased scalability.
- Reliable operation during network interruptions.

## Challenges

- Internet connectivity problems.
- Cybersecurity risks.
- Higher implementation cost.
- Complex system integration.

## Final Conclusion
The modified smart hospital design combines real-time operating systems, mobile operating systems, clustered servers and distributed cloud services.

This approach provides patient safety, security, reliability and scalability.