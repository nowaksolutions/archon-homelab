<p align="center">
  <img src="assets/archon-phys-topo.jpg" alt="ARCHON Physical Topology" width="850">
</p>

<h2 align="center">Operational Architecture (CySA+ Aligned)</h2>

<p align="center">
  This environment is designed to simulate enterprise security operations with a focus on monitoring,
  detection, and response. The architecture aligns with CySA+ objectives and incorporates principles
  from NIST CSF, NIST SP 800-53, and NIST SP 800-61 to support real-world defensive workflows.
</p>

<br>

<h3>Network Segmentation (Control & Containment)</h3>

<p>
<b>WAN</b> - External untrusted network used to simulate inbound threat activity and reconnaissance<br>
<b>LAN</b> - Internal production-like environment hosting user endpoints and domain services<br>
<b>MGMT</b> - Restricted administrative network for secure management of infrastructure components<br>
<b>LAB</b> - Isolated adversary simulation environment for controlled attack testing and validation
</p>

<p>
Segmentation is enforced through firewall policy and virtual network isolation to align with NIST 800-53
controls related to boundary protection and network segmentation. This reduces attack surface and limits
lateral movement during simulated compromise scenarios.
</p>

<br>

<h3>Core Security Components (Visibility & Detection)</h3>

<p>
<b>Firewall</b> - Implements boundary defense, traffic inspection, and access control enforcement<br>
<b>SIEM</b> - Aggregates and correlates logs to support detection, alerting, and analysis (NIST 800-137)<br>
<b>Domain Controller</b> - Provides identity services and generates authentication logs for monitoring<br>
<b>Raspberry Pi Monitoring Node</b> - Supports continuous system health monitoring and telemetry collection<br>
<b>NAS</b> - Stores logs and artifacts for analysis, retention, and incident review<br>
<b>Virtual Systems</b> - Generate realistic user, server, and attacker behavior for detection use cases
</p>

<br>

<h3>Detection & Monitoring Strategy (CySA+ Focus)</h3>

<p>
The environment supports continuous monitoring and threat detection through centralized log collection
and analysis. Events from endpoints, authentication systems, and network activity are forwarded to the
SIEM to enable correlation and anomaly detection.
</p>

<p>
Detection use cases include identification of brute force attempts, unauthorized access, privilege escalation,
and suspicious network behavior. This aligns with CySA+ objectives around log analysis, threat detection,
and behavioral monitoring.
</p>

<br>

<h3>Traffic Flow & Analysis</h3>

<p>
All inbound traffic is inspected at the firewall prior to entering internal segments. East-west traffic between
network zones is restricted and monitored to detect abnormal communication patterns. Administrative access
is isolated within the MGMT network to reduce exposure of critical systems.
</p>

<p>
This design supports traffic analysis and network-based detection strategies consistent with NIST guidance
on continuous monitoring and anomaly detection.
</p>

<br>

<h3>Incident Response Alignment</h3>

<p>
The lab environment supports incident response workflows aligned with NIST SP 800-61, including:
</p>

<p>
<b>Detection & Analysis</b> - Identification of suspicious events through SIEM correlation<br>
<b>Containment</b> - Use of segmentation and firewall controls to isolate affected systems<br>
<b>Eradication & Recovery</b> - Simulated remediation and system restoration processes<br>
<b>Post-Incident Activity</b> - Log review and documentation for lessons learned
</p>

<br>

<h3>Security Principles Applied</h3>

<p>
<b>Defense in Depth</b> - Multiple layers of controls across network and systems<br>
<b>Least Privilege</b> - Restricted access to minimize risk exposure<br>
<b>Segmentation</b> - Isolation of network zones to limit lateral movement<br>
<b>Continuous Monitoring</b> - Centralized visibility aligned with NIST 800-137
</p>

<br>

<h3>Operational Use Cases</h3>

<p>
Security log analysis and correlation<br>
Threat detection and anomaly identification<br>
Brute force and authentication attack monitoring<br>
Lateral movement simulation and detection<br>
Firewall rule validation and traffic inspection<br>
Incident response workflow development and testing
</p>
