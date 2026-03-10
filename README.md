# Network-Security-Analysis

📌 Overview

This project demonstrates practical network security analysis using only built-in tools available in Kali Linux.
The focus is on discovering network assets, monitoring traffic, and identifying suspicious behavior using packet inspection and network scanning.

🎯 Objectives

Discover devices on a network
Identify open ports and running services
Capture and inspect live network traffic
Detect suspicious communication patterns
Document security findings

🛠️ Tools Used

Kali Linux— Security-focused operating system

Nmap — Network discovery & port scanning

Wireshark — Network protocol & packet analysis

🧪 Project Workflow

1️⃣ Lab Setup

Used Kali Linux as the testing environment
Connected to a local network / virtual lab
Ensured legal and authorized testing only

2️⃣ Network Discovery (Nmap)

Identified active hosts on the network
Scanned open ports and exposed services
Detected service versions

3️⃣ Traffic Capture (Wireshark)

Monitored live network traffic
Captured packets for deeper inspection
Filtered traffic by protocol and IP address

4️⃣ Traffic Analysis

Inspected TCP/IP communication
Observed DNS requests and responses
Reviewed HTTP traffic patterns
Distinguished normal vs suspicious behavior

5️⃣ Security Findings

Identified unnecessary open ports
Detected unencrypted communications
Observed unusual connection attempts

6️⃣ Reporting

Documented scan results
Captured packet evidence
Provided mitigation suggestions

📂 Project Structure

network-security-analysis/

├── nmap-scans/           # Scan result files

├── wireshark-captures/   # .pcap packet capture files

├── screenshots/          # Tool output images

├── report/               # Final findings

└── README.md             # Project documentation

▶️ How to Run

Start Network Scan

nmap -sn 192.168.1.0/24

Service & Version Detection

nmap -sV target-ip

Full Port Scan

nmap -p- target-ip

Capture Network Traffic

wireshark

Select active network interface

Start capture

Save file as .pcap

Useful Wireshark Filters

http

dns

ip.addr == target-ip

tcp.flags.syn == 1

📊 Key Learnings

Hands-on network reconnaissance
Packet-level traffic investigation
Protocol behavior understanding
Identifying security misconfigurations
Practical cybersecurity analysis workflow

🚨 Sample Findings

Devices with multiple open ports
Services running outdated versions
Plain-text traffic (no encryption)
Repeated connection attempts from unknown hosts

🛡️ Mitigation Recommendations

Close unused ports
Disable unnecessary services
Use encrypted protocols (HTTPS, SSH)
Configure firewall rules
Monitor network regularly

👨‍💻 Author

Kishore Dey : 
IT & Cybersecurity Enthusiast | Ethical Hacking Learner

📜 Disclaimer :
This project is for educational purposes only.
All testing was performed in an authorized lab environment.
