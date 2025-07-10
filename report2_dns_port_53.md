# Report 2: DNS Port 53 Unreachable

## Part 1: Summary of the Problem
As part of the DNS protocol, the UDP protocol was used to contact the DNS server to retrieve the IP address for the domain name `facebook.com`. The ICMP protocol responded with an error, indicating issues contacting the DNS server.

UDP messages from the browser to the DNS server were logged in the first two lines of each event. ICMP error responses appeared in lines 3 and 4 with the message: "udp port 53 unreachable". Since port 53 is used for DNS traffic, this suggests an issue with the DNS server. The + symbol and "A?" in the DNS query further confirm DNS protocol activity.

## Part 2: Analysis of the Data
The incident occurred today at 1:24 PM. Customers reported seeing the error “destination port unreachable” when accessing `facebook.com`. The cybersecurity team ran a tcpdump analysis and confirmed that DNS port 53 was unreachable.

Next steps include verifying whether the DNS server is down or if a firewall is blocking port 53. A DoS attack or misconfiguration is suspected.
