# Active Directory Splunk Lab Using VirtualBox VMs
## Introduction
In this lab, I build a Active Directory environment with a Splunk server to ingest logs from AD hosts. I used a Kali Linux VM to conduct attacks against the AD environment, and be able to detect malicious activity against our network using Splunk. The key lessons learned through this lab are:
- Installing various operating systems as Virtual Machines (VMs) using VirtualBox, and configuring the network adapters so that the different machines can communicate with one another.
- Configuring servers:
  - Configuring AD Domain Controller, add groups/users, and domain join a Windows host.
  - Configuring Splunk server, and install Splunk agents on Domain Controller and hosts to ingest logs.
- Conduct attacks against AD environment from Kali VM to inspect activity in Splunk.
- Install Atomic Red Team on Windows host to generate telemetry on various MITRE ATT&CK adversary techniques and tactics.

## Lab Topology
This lab consists of four hosts:
- 2022 Windows Server: Domain Controller for the network's domain.
- Windows 10: Workstation inside the network domain.
- Splunk Server (Ubuntu 22.04): Splunk server ingesting logs from Domain Controller and Windows host.
- Kali Linux: Host used to conduct attacks against Windows host.
<p align="center" width="100%">
    <img src="https://github.com/EdgarAcuna8/VB-Active-Directory-Splunk/assets/146898815/6411000b-ef2f-47d2-9ef9-db0abe8ebac7">
</p>
