<p align="center">
  <img src="assets/dc-deployment-banner.png" alt="Domain Controller Deployment Banner" width="100%">
</p>

---

## 🔷 Overview

This project focuses on the deployment and secure configuration of a Windows Server Domain Controller within the ARCHON homelab environment. The goal is to simulate a real-world enterprise identity infrastructure while maintaining strong security boundaries and controlled access.

The Domain Controller provides centralized authentication, authorization, and directory services for lab-connected systems, forming the foundation for identity-driven security operations.

---

## 🔷 Core Functions

Active Directory Domain Services (AD DS)  
Centralized identity management for users, systems, and resources within the environment  

Authentication (Kerberos)  
Secure ticket-based authentication mechanism for domain-joined systems  

Authorization (Group Policy)  
Policy-based access control and configuration enforcement across endpoints  

DNS Integration  
Internal name resolution supporting domain operations and service discovery  

---

## 🔷 Architecture Context

The Domain Controller is deployed within a segmented lab network to replicate enterprise design principles.

- Isolated within a controlled network segment  
- Serves as the authoritative identity source for domain-joined systems  
- Integrated with internal DNS for service resolution  
- Supports endpoint authentication and policy enforcement  
- Logs security-relevant events to centralized monitoring systems  

This design reinforces separation of duties and reduces unnecessary exposure across network boundaries.

---

## 🔷 Security Design & Hardening Approach

This deployment emphasizes secure configuration aligned with industry best practices and defensive principles.

### Identity & Access Control

Principle of Least Privilege  
Administrative access is restricted and controlled to minimize risk  

Controlled Administrative Usage  
Privileged operations are separated from standard user activity  

Account Policies  
Lockout thresholds and credential policies are enforced to mitigate brute-force attempts  

---

### Authentication Security

Kerberos-First Approach  
Modern authentication protocols are prioritized over legacy mechanisms  

Credential Protection  
Measures are in place to reduce exposure of sensitive authentication material  

---

### System Hardening

Reduced Attack Surface  
Unnecessary roles and services are not enabled  

Patch Management  
System updates are applied regularly to address known vulnerabilities  

Secure Baseline Alignment  
Configuration follows Microsoft and NIST-informed hardening strategies  

---

### Network Security

Segmentation Enforcement  
The Domain Controller is not directly exposed to untrusted networks  

Controlled Access Paths  
Traffic to and from the system is restricted through firewall policy  

---

### Monitoring & Visibility

Audit Logging Enabled  
Security-relevant events are captured for analysis  

Centralized Log Forwarding  
Logs are integrated into a monitoring pipeline for visibility and detection  

---

## 🔷 Key Takeaways

- Identity infrastructure is a primary security boundary in enterprise environments  
- Misconfiguration of Active Directory can introduce significant risk  
- Segmentation and access control are critical to protecting authentication systems  
- Logging and monitoring are essential for detecting abnormal activity  

---

## 🔷 Lessons Learned

- Proper DNS configuration is critical for domain functionality  
- Authentication issues often trace back to network or name resolution problems  
- Segmentation must be carefully validated across Layer 2 and Layer 3  
- Maintaining management access during configuration changes is essential  

---

## 🔷 Future Enhancements

- Group Policy expansion for endpoint hardening  
- Integration with SIEM for advanced detection use cases  
- Role-based access model refinement  
- Expansion into multi-tier or multi-domain architecture  

---
