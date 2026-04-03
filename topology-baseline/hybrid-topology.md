<p align="center">
  <img src="assets/archon-phys-topo.jpg" alt="ARCHON Physical Topology" width="850">
</p>

<p align="center">
  <em>Segmented homelab architecture with firewall enforcement, SIEM visibility, and monitored infrastructure nodes</em>
</p>

<h2 align="center">Architecture Overview</h2>

<p align="center">
  This environment is a segmented homelab designed to simulate real-world enterprise network operations,
  security monitoring, and controlled traffic flow across multiple network zones.
</p>

<br>

<h3>Network Segmentation</h3>

<p>
<b>WAN</b> - External untrusted network representing internet traffic<br>
<b>LAN</b> - Internal network hosting user systems and core services<br>
<b>MGMT</b> - Restricted network for administrative access and system control<br>
<b>LAB</b> - Isolated environment for testing, attack simulation, and validation
</p>

<br>

<h3>Core Components</h3>

<p>
<b>Firewall</b> - Enforces segmentation, filters traffic, and controls inter-network communication<br>
<b>SIEM</b> - Centralizes logs for monitoring, detection, and analysis<br>
<b>Domain Controller</b> - Handles authentication, authorization, and policy management<br>
<b>Raspberry Pi Monitor</b> - Tracks system health and supports lightweight monitoring<br>
<b>NAS</b> - Stores logs, backups, and lab data<br>
<b>Managed Switch</b> - Supports internal segmentation and network distribution<br>
<b>Virtual Machines</b> - Simulate endpoints, servers, and attacker systems
</p>

<br>

<h3>Traffic Flow</h3>

<p>
All inbound traffic is inspected at the firewall before entering internal networks.
Communication between segments is restricted and monitored to reduce unauthorized access
and limit lateral movement. Administrative access is isolated to the MGMT network.
</p>

<br>

<h3>Security Approach</h3>

<p>
<b>Defense in Depth</b> - Layered controls across network and systems<br>
<b>Least Privilege</b> - Restricted access to minimize exposure<br>
<b>Segmentation</b> - Isolates systems to reduce risk and contain threats<br>
<b>Centralized Monitoring</b> - Enables visibility across all components
</p>

<br>

<h3>Use Cases</h3>

<p>
Log analysis and correlation<br>
Brute force and anomaly detection<br>
Lateral movement simulation<br>
Firewall rule validation<br>
Incident response practice
</p>
