# Report 1: HTTPS Port 443 Unreachable

## Part 1: Summary of the Problem
The network protocol analyzer logs indicate that port 443 is unreachable when attempting to access the secure employee background check website. Port 443 is normally used for HTTPS traffic. This may indicate a problem with the web server or the firewall configuration. It is possible that this is an indication of a malicious attack on the web server.

## Part 2: Analysis of the Data
The incident occurred earlier this morning when the HR team reported that they could not access the background check web portal. The network security team responded and ran tests using the tcpdump tool. Logs revealed that port 443 (used for HTTPS) was not reachable.

Next steps include checking the firewall configuration to see if port 443 is blocked and contacting the system administrator for the web server to look for signs of an attack. The HR team suspects that a recent hire might be trying to block background checks, and the security team suspects this individual may have launched an attack on the web server.
