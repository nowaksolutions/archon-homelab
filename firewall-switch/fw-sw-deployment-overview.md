# 🔐 Firewall and Switch Deployment with VLAN Segmentation

---

## 📌 Objective

Designed and deployed an integrated firewall and managed switch architecture to simulate enterprise-grade network segmentation and traffic control.

The environment leverages Layer 2 switching for VLAN segmentation, 802.1Q trunking for multi-VLAN transport, and Layer 3 firewall routing for inspection and policy enforcement.

This lab demonstrates how switching, trunking, and firewall controls operate together to define secure network boundaries and regulate traffic flow across the OSI model.

---

## 🧠 Architecture Overview

| Component        | Function |
|-----------------|----------|
| Managed Switch   | VLAN segmentation and Layer 2 frame forwarding |
| Firewall         | Inter-VLAN routing, inspection, and policy enforcement |
| Trunk Link       | Tagged VLAN transport between switch and firewall |
| Access Ports     | Endpoint VLAN assignment via PVID |
| VLAN Interfaces  | Logical gateways for segmented networks |

---

## ⚙️ Key Focus Areas

- VLAN segmentation aligned to functional roles such as personal, lab, and monitoring networks
- 802.1Q trunking between firewall and switch to carry multiple VLANs over a single uplink
- Separation of trunk and access ports to enforce deterministic switching behavior
- Ingress classification using PVID to assign untagged frames to correct VLANs
- Firewall acting as the Layer 3 gateway for all VLANs
- Centralized inter-VLAN routing to ensure inspection and policy enforcement
- Stateful firewall rules governing east-west and north-south traffic
- Segmented DHCP scope provisioning per VLAN
- Validation of traffic flow across OSI Layers 2 through 4

---

## 🔍 Packet Flow Walkthrough


[Endpoint Device]
   ↓ (untagged Ethernet frame)
[Switch Access Port]
   → VLAN assigned via PVID
   ↓ (frame tagged with VLAN ID)
[Switch Trunk Port - 802.1Q]
   ↓
[Firewall VLAN Interface]
   → Routing decision made
   → Firewall policy evaluated
   ↓
[Destination VLAN or External Network]

Return traffic follows the same path in reverse with stateful inspection applied.

---

## 🧪 Lessons Learned

- Layer 2 and Layer 3 alignment is critical, VLAN tagging on the switch must match firewall interface configuration or traffic fails silently
- Trunk configuration is foundational, improper tagging or VLAN allowance breaks segmentation entirely
- Access ports require correct PVID assignment or endpoints are placed into incorrect broadcast domains
- Firewall must maintain a dedicated interface for each VLAN carried across the trunk
- Restricting VLANs on trunk ports reduces attack surface and enforces tighter control
- Default or native VLAN configurations introduce unnecessary risk and should be minimized
- DHCP may function even when routing is broken due to broadcast behavior, requiring deeper validation
- Firewall rules only apply after traffic reaches the correct interface, pre-routing failures are typically Layer 2 issues
- Maintaining management access during configuration changes is essential to prevent lockout

---

## 🛡️ Security and Framework Alignment

| Framework        | Implementation Alignment |
|-----------------|--------------------------|
| NIST SP 800-41  | Firewall-based boundary protection and traffic control |
| NIST SP 800-53  | SC-7 boundary protection and AC-4 information flow enforcement |
| NIST SP 800-115 | Validation through structured testing and troubleshooting |
| NIST CSF        | Network segmentation, access control, and monitoring readiness |

The architecture enforces least privilege at the network level and reduces lateral movement, aligning with zero trust design principles.

---

## 🎯 Outcome

Deployed a segmented and trunked network architecture capable of supporting:

- Controlled inter-VLAN communication through firewall enforcement
- Traffic inspection, logging, and monitoring integration
- Realistic attack simulation and detection workflows
- Scalable expansion for SIEM, IDS/IPS, and endpoint monitoring tools

This lab establishes a strong foundation for network security operations, threat detection, and infrastructure hardening.
