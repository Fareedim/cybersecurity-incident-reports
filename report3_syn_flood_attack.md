# Report 3: SYN Flood DoS Attack – Web Server Timeout

## Section 1: Identifying the Type of Attack

One potential explanation for the website’s connection timeout error message is a **Denial-of-Service (DoS) attack**.  
The logs show that the **web server stops responding after being overloaded with SYN packet requests**.  
This is a type of DoS attack called a **SYN flood**.

## Section 2:  How the Attack Caused the Malfunction

When website visitors try to establish a connection with the web server, a **TCP three-way handshake** occurs:

1. A **SYN** packet is sent from the source to the destination.
2. The destination replies with a **SYN-ACK** and reserves system resources.
3. The source responds with an **ACK**, completing the handshake.

In a **SYN flood attack**, a malicious actor sends a large number of **SYN packets in rapid succession**, but never completes the handshake.  
This **exhausts the server’s ability to allocate resources**, leaving it unable to handle legitimate connection requests.  

As a result, visitors receive a **connection timeout** error when trying to access the site.

