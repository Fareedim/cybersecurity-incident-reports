# Cybersecurity Incident Reports Portfolio

This repository contains sample incident reports.

##  Reports Included

### 1. HTTPS Port 443 Unreachable - Background Check Web Portal
- **Incident:** HR team unable to access secure background check portal
- **Analysis Tool:** tcpdump
- **Protocol:** HTTPS 
- **Key Finding:** Port 443 unreachable; possible misconfiguration or targeted attack
- **Status:** Under investigation

### 2. DNS Port 53 Unreachable - Website Access Issue
- **Incident:** Customers unable to reach `facebook.com`
- **Analysis Tool:** tcpdump
- **Protocols:** UDP and ICMP
- **Key Finding:** ICMP message "udp port 53 unreachable" suggests DNS server issue
- **Status:** DNS or firewall issue suspected; further investigation required

---

##  Tools Used
- tcpdump
- Basic packet analysis (ICMP, UDP, DNS)

