<h2 align="center">Topology Overview</h2>

<p align="center">
  This hybrid topology represents a segmented homelab environment combining physical infrastructure
  and virtual systems to simulate controlled network operations and security-focused traffic flow.
</p>

<p align="center">
  <img src="assets/archon-phys-topo.jpg" alt="ARCHON Physical Topology" width="850">
</p>

<br>

<h3>Network Flow</h3>

<p>
Internet traffic enters through the ISP modem/router and is passed to the firewall, which serves as the
primary control point for traffic filtering, NAT, and segmentation enforcement. Traffic is then distributed
through a managed switch to connected systems and services.
</p>

<br>

<h3>Core Infrastructure</h3>

<p>
<b>ISP Modem/Router</b> - Provides external connectivity and upstream network access<br>
<b>Firewall (Protectli Vault)</b> - Enforces traffic filtering, NAT, and segmentation policies<br>
<b>Managed Switch (NETGEAR GS308EP)</b> - Distributes network connectivity and supports VLAN segmentation<br>
<b>UPS</b> - Maintains power continuity and protects critical infrastructure
</p>

<br>

<h3>Connected Systems</h3>

<p>
<b>Personal Workstation</b> - Primary user system generating normal traffic and administrative access<br>
<b>NAS</b> - Central storage for backups, logs, and system data<br>
<b>Domain Controller</b> - Provides AD, DNS, DHCP, and identity services<br>
<b>SIEM Server</b> - Collects and analyzes logs for monitoring and visibility<br>
<b>Windows Endpoint</b> - Simulated client system for user activity and logging<br>
<b>Attack Node (Kali Linux)</b> - Generates controlled adversarial activity for testing<br>
<b>Monitoring Node (Raspberry Pi)</b> - Collects telemetry and supports system monitoring
</p>

<br>

<h3>Segmentation Model</h3>

<p>
Network segmentation is enforced at the firewall and supported by switch-level VLAN configuration.
This separates user systems, management functions, and testing environments to control traffic flow
and reduce unintended access between systems.
</p>

<br>

<h3>Design Intent</h3>

<p>
The topology is structured to provide visibility into network activity while maintaining controlled
interaction between systems. It supports realistic traffic patterns, administrative workflows, and
isolated testing within a single integrated environment.
</p>
