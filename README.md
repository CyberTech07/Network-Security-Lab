# Network Security Lab

## Project Overview
This project demonstrates the setup of a virtual network security lab using VMware Workstation 17 Player. I segmented traffic with VLANs (VLAN10 for Ubuntu and VLAN20 for Kali Linux) and configured pfSense as a firewall and router. I deployed Suricata IDS to detect intrusions and tested the network with pings and an Nmap scan.

## Key Features
- *VLAN Configuration*: Set up VLAN10 (192.168.10.100 for Ubuntu) and VLAN20 (192.168.20.100 for Kali) on pfSense.
- *Manual DHCP*: Configured DHCP manually on OPT1 and OPT2 interfaces.
- *Firewall Rules*: Added ICMP rules on OPT1 to allow ping traffic.
- *Intrusion Detection*: Enabled Suricata with Emerging Threats rules (Exploits, Malware, Scan) and detected an Nmap scan ("ET SCAN Nmap Scripting Engine Scan").
- *Backup*: Created and verified a pfSense configuration backup (config.xml).

## Tools Used
- VMware Workstation 17 Player
- pfSense
- Suricata
- Kali Linux
- Ubuntu
- Nmap
- VLANs
- TCP/IP
- XML

## Screenshots
- [Interfaces Assignment](pfSense_Interfaces_Phone.jpg): Captures the pfSense Interfaces > Assignments page, showcasing the configuration of WAN, OPT1 (VLAN10 with IP 192.168.10.1), and OPT2 (VLAN20 with IP 192.168.20.1). This setup ensures network segmentation for Ubuntu and Kali Linux VMs, a core component of the lab established on July 04, 2025.
- [Suricata Interfaces](pfSense_Suricata_Interfaces_Phone.jpg): Displays the Suricata > Interfaces configuration, highlighting the enabling of IDS on WAN, OPT1, and OPT2 interfaces. Configured with Emerging Threats rules (Exploits, Malware, Scan) on May 12, 2025, this setup monitors network traffic for intrusions, validated by an Nmap scan detection.
- [Firewall Rule OPT1](pfSense_Firewall_OPT1_Phone.jpg): Shows the Firewall > Rules page for OPT1, featuring an ICMP rule allowing ping traffic from VLAN10 (192.168.10.0/24) to any destination. Implemented on July 04, 2025, this rule enabled successful ping tests from the Ubuntu VM, demonstrating network accessibility.
- [Backup Restore](pfSense_Backup_Phone.jpg): Illustrates the Diagnostics > Backup & Restore page, confirming the download of the pfSense configuration backup (config.xml) at 10:37 AM WAT on July 04, 2025. This step ensures the lab’s settings are preserved for future reference or restoration.

## Achievements
Successfully delivered a secure, segmented network with functional IDS detection through persistent troubleshooting.

## Contact
Feel free to reach out for questions or collaboration!
