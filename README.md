# Man-in-the-Middle
MITM Attack Simulation & Analysis
Title: Man-in-the-Middle (MITM) Vulnerability Assessment
1. Simulation Overview Using Wireshark and ARP spoofing techniques, I simulated an interception attack between a client machine and a local gateway. The goal was to evaluate the risk of data exposure on unencrypted channels.
2. Log Analysis & Findings * Protocol Vulnerability: The capture identified traffic using HTTP (Port 80).
Data Exposure: Because the protocol is unencrypted, "Packet Sniffing" allowed for the reconstruction of full TCP streams.
Evidence: Sensitive credentials (usernames/passwords) were identified in cleartext within the HTTP POST requests.
3. Mitigation Recommendations * Universal Encryption: Transition all local services to HTTPS/TLS 1.3.
Port Security: Implement DHCP snooping and Dynamic ARP Inspection on network switches to prevent the redirection of traffic.

