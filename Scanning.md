# Network Scanning with Zenmap

## Cybersecurity & Ethical Hacking – Practical Project

**Author:** W.P. Nethmi Bhayogya  
**Date:** 17 November 2026  
**Tool:** Zenmap (Nmap GUI)  
**Operating System:** Windows 10

---

## 1. Project Overview

This project demonstrates network discovery and host identification using Zenmap, the graphical user interface for Nmap.

The practical was conducted as part of the Cybersecurity & Ethical Hacking program at Networkwalks. The objective was to identify the local network configuration, discover active hosts, identify IP and MAC addresses, and visualize the discovered network topology.

All scanning activities were performed on my own local network for educational purposes.

## 2. Objectives

- Identify the local IP address and subnet configuration.
- Understand the purpose of network scanning.
- Discover active hosts within the local network.
- Identify IP and MAC addresses of discovered devices.
- Understand Ping Scanning using Nmap.
- Generate and analyze a network topology using Zenmap.

## 3. Tools and Technologies

| Tool | Purpose |
|---|---|
| Windows 10 | Operating system |
| Windows CMD | Identify network configuration using `ipconfig` |
| Zenmap | Graphical interface for Nmap |
| Nmap | Network discovery and scanning engine |

## 4. Network Configuration

The Windows `ipconfig` command was used to identify the local network configuration.

| Configuration | Value |
|---|---|
| IPv4 Address | 192.168.146.64 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | 192.168.146.171 |
| Network Address | 192.168.146.0/24 |

## 5. Network Scanning

### 5.1 Scan Configuration

The following configuration was used in Zenmap:

- **Target:** `192.168.146.0/24`
- **Profile:** Ping Scan
- **Command:** `nmap -sn 192.168.146.0/24`

The `-sn` option performs host discovery without conducting a port scan.

### 5.2 Scan Results

The scan discovered two active hosts within the specified subnet.

| IP Address | Status |
|---|---|
| 192.168.146.171 | Host is up |
| 192.168.146.64 | Host is up |

**Scan summary:**
- IP addresses scanned: 256
- Active hosts discovered: 2
- Scan duration: 10.29 seconds

### 5.3 MAC Address Identification

The scan identified the following MAC address:

`FE:A2:C6:C8:BD:CD`

The MAC address vendor was not identified in the Nmap output.

### 5.4 Network Topology

The Zenmap Topology section was used to visualize the discovered hosts and their network relationships.

The topology view was reviewed and saved as evidence.

## 6. Key Findings

1. Successfully identified the local IPv4 configuration.
2. Identified the `/24` subnet containing 256 IPv4 addresses.
3. Discovered two active hosts using Ping Scan.
4. Retrieved a MAC address for a discovered host.
5. Generated a network topology using Zenmap.

## 7. Security Considerations

Network scanning is an important activity in cybersecurity because it helps administrators identify active devices and understand network exposure.

Regular network discovery can help organizations:
- Identify unknown devices.
- Maintain an accurate network inventory.
- Understand their network structure.
- Detect unexpected devices for further investigation.

Scanning should only be performed on networks where appropriate authorization has been obtained.

## 8. Conclusion

Through this practical exercise, I gained hands-on experience with network discovery using Zenmap and Nmap.

I learned how to identify local network configurations, perform Ping Scans, discover active hosts, examine MAC address information, and visualize network topology.

This practical helped me understand the importance of network scanning as an initial step in cybersecurity assessments and network security monitoring.

## 9. Evidence

Screenshots documenting the practical activities are available in the `Screenshots` directory.

- Windows IP configuration
- Zenmap Ping Scan configuration
- Discovered hosts and scan output
- Network topology visualization

---

**Program:** Cybersecurity & Ethical Hacking  
**Training Organization:** Networkwalks  
**Author:** W.P. Nethmi Bhayogya
