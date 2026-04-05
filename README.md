<p align="center">
  <img src="assets/archon-lp-banner.png" alt="ARCHON Homelab Banner" width="100%">
</p>

<h1 align="center">A.R.C.H.O.N Homelab</h1>

<p align="center">
  Advanced Reconnaissance & Control Host Operations Network
</p>

<p align="center">
  <i>Structured cybersecurity lab built for disciplined learning, operational awareness, and real-world skill development.</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active%20Development-blue">
  <img src="https://img.shields.io/badge/Focus-SOC%20%7C%20CySA%2B-red">
  <img src="https://img.shields.io/badge/Environment-Segmented%20Lab-black">
  <img src="https://img.shields.io/badge/Stack-Windows%20%7C%20Linux%20%7C%20SIEM-blueviolet">
</p>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<p align="center">
  <i>I want to give a quick thank you to my friend Reece Niemuth for being a mentor throughout this process and for the design inspiration behind this lab. Your guidance and perspective have played a major role in shaping what I’m building here, and I truly appreciate it.</i>
</p>

<p align="center">
  <a href="https://github.com/ReeceNiemuth" target="_blank">
    <img src="https://img.shields.io/badge/Mentor-Reece%20Niemuth-blue?style=for-the-badge&logo=github">
  </a>
</p>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<h2>🔎 Quick Snapshot</h2>

<p>
<strong>Purpose:</strong> Hands-on SOC and security engineering training environment<br>
<strong>Focus:</strong> Threat detection, log analysis, vulnerability assessment, and system integration<br>
<strong>Stack:</strong> Windows, Linux, SIEM, Active Directory, Firewall, Raspberry Pi<br>
<strong>Approach:</strong> Structured, disciplined, and process-oriented
</p>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<h2>🖥️ Physical Lab Environment</h2>

<p align="center">
  <img src="assets/homelab-photo.jpg" alt="ARCHON Homelab Setup" width="85%">
</p>

<p align="center">
  <i>Physical deployment of the ARCHON homelab environment supporting segmented networking, monitoring, and system integration.</i>
</p>

<h2>🎯 Purpose & Development Approach</h2>

<p>
This homelab is a continuously evolving environment built to develop practical cybersecurity and IT operations capability through hands-on implementation. The objective is not simply to assemble systems, but to understand how infrastructure behaves, how security controls are enforced, and how activity is detected, analyzed, and escalated in an operational setting.
</p>

<p>
The environment is intentionally structured around core security operations concepts, including <strong>network segmentation</strong>, <strong>centralized logging</strong>, <strong>continuous monitoring</strong>, <strong>endpoint visibility</strong>, and <strong>identity management</strong>. Each component is deployed with purpose and integrated to support realistic workflows such as alert triage, investigation, and response validation.
</p>

<p>
This lab is developed with reference to established security frameworks such as the NIST Cybersecurity Framework (CSF) and supporting guidance from NIST Special Publications, emphasizing structured control implementation, monitoring, and assessment practices.
</p>

<p>
My approach is influenced by prior military experience, emphasizing disciplined troubleshooting, escalation awareness, and structured analysis. This translates into building systems with clear boundaries, maintaining visibility across the environment, and approaching problems with a repeatable and methodical process.
</p>

<p>
This lab serves as a training ground to bridge theory and execution while reinforcing the mindset and technical foundations required for real-world cybersecurity roles.
</p>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<h2>📚 Training Objectives</h2>

<p>
The environment is designed to build capability through direct interaction with systems, logs, and security controls across multiple domains.
</p>

<p>
<strong>Digital Forensics</strong><br>
Analysis of system artifacts, event timelines, and evidence collection across Windows and Linux systems
</p>

<p>
<strong>Threat Hunting & Log Analysis</strong><br>
Identification of anomalies and indicators of compromise through SIEM workflows
</p>

<p>
<strong>Security & Network Engineering</strong><br>
Design and enforcement of segmented architecture and controlled traffic flow
</p>

<p>
<strong>Endpoint Detection & Response (EDR)</strong><br>
Monitoring endpoint behavior and understanding detection and response mechanisms
</p>

<p>
<strong>Aggregation & Integration</strong><br>
Centralizing and correlating logs across multiple systems
</p>

<p>
<strong>API Interaction & Automation</strong><br>
Integrating tools and automating workflows through API-based communication
</p>

<p>
<strong>Active Directory</strong><br>
Managing authentication, authorization, and policy enforcement in a domain environment
</p>

<p>
<strong>Cross-Platform Administration</strong><br>
Operating across Windows and Linux environments to understand differences in system behavior and security controls
</p>

<p>
<strong>Vulnerability Assessment</strong><br>
Identification, validation, and prioritization of system weaknesses through scanning and analysis
</p>

<p>
<strong>System Hardening & Baselines</strong><br>
Applying and validating secure configuration standards aligned with industry benchmarks
</p>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<h2>🧱 Core Infrastructure</h2>

<table>
<tr>
<td><strong>ISP Gateway</strong></td>
<td>External connectivity entry point into the lab environment</td>
</tr>

<tr>
<td><strong>Firewall</strong></td>
<td>Segmentation enforcement, access control, and traffic inspection between network zones</td>
</tr>

<tr>
<td><strong>SIEM</strong></td>
<td>Centralized logging, event correlation, and continuous monitoring</td>
</tr>

<tr>
<td><strong>Virtual Machines</strong></td>
<td>Windows and Linux systems used for endpoint simulation, attack emulation, and log generation</td>
</tr>

<tr>
<td><strong>Domain Controller</strong></td>
<td>Centralized identity management, authentication, and policy enforcement</td>
</tr>

<tr>
<td><strong>Raspberry Pi Monitoring Node</strong></td>
<td>Lightweight system providing health monitoring and supplemental visibility</td>
</tr>

<tr>
<td><strong>NAS</strong></td>
<td>Centralized storage for logs, configurations, and retained data</td>
</tr>

<tr>
<td><strong>UPS</strong></td>
<td>Power continuity and protection for system stability</td>
</tr>
</table>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<h2>⚙️ Operational Focus</h2>

<p>
This environment is designed to simulate real-world security operations rather than isolated technical exercises.
</p>

<p>
Primary focus areas include generating and analyzing logs, identifying abnormal behavior, validating detections, performing vulnerability assessments, and understanding how systems interact during both normal operation and potential security events.
</p>

<p>
Emphasis is placed on <strong>visibility</strong>, <strong>control</strong>, and <strong>repeatability</strong>, ensuring that actions taken within the lab can be understood, documented, and refined over time.
</p>

<blockquote>
<strong>Note:</strong> This lab is actively developed and continuously refined as part of ongoing cybersecurity training and skill progression.
</blockquote>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<h2>🌐 Topology</h2>

<p>
Baseline network design, segmentation layout, and system relationships are documented in the <code>topology-baseline</code> directory.
</p>

<p align="center">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</p>

<h2>📈 Status</h2>

<p>
Active development. Additional monitoring, integrations, automation, and detection capabilities are continuously being implemented.
</p>
