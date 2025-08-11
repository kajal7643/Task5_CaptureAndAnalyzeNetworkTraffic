Task 5 – Capture and Analyze Network Traffic Using Wireshark  
Objective  
The goal of this task was to capture live network packets with Wireshark, filter them by protocol, and identify basic protocols and traffic types to improve packet analysis skills and protocol awareness.  
Tools Used  
Wireshark vX.X (Free, Open Source)  

Steps Performed  
 Installed Wireshark on my system.  
 Launched Wireshark and selected the active network interface (Wi-Fi).  
 Started live capture to monitor network activity.  
 Generated network traffic by:  
- Visiting multiple websites in a web browser.  
- Pinging an external server (ping google.com).  
 Stopped the capture after about 1 minute.  
 Applied filters to view specific protocols (e.g., tcp, arp, tls).  
 Saved the capture file as .pcapng.  
 Analyzed packets and noted details of at least three different protocols.  
Protocols Identified  
TCP (Transmission Control Protocol)  
- A reliable, connection-oriented protocol.  
- Observed in packet exchanges between my system and web servers.  
- Example: TCP ACK packets showing sequence and acknowledgment numbers.  

TLSv1.3 (Transport Layer Security)  
- Offers encrypted communication for HTTPS traffic.  
- Seen as "Application Data" packets.  
- Example: TLS handshake and encrypted web data from visiting websites.  

ARP (Address Resolution Protocol)  
- Resolves IP addresses to MAC addresses in local network communication.  
- Example: ARP request to find the MAC address of a local IP.  

Sample Packet Details  
TCP Packet:  
```
Src IP: 2401:4900:8813:1d51::  
Dst IP: 2404:6800:4009:827::  
Seq: 33117, Ack: 283392, Len: 0  
```  
TLSv1.3 Packet:  
```
Protocol: TLSv1.3  
Content Type: Application Data  
Length: 965 bytes  
```  
ARP Request:  
```
Who has 192.168.1.73? Tell 192.168.1.1  
```  
Outcome  
 Successfully captured live traffic using Wireshark.  
 Identified and filtered multiple protocols.  
 Understood how TCP/IP layers interact during normal network operations.  
 Gained hands-on experience in protocol analysis and the basics of network troubleshooting.  

Files in This Repository  
task5_capture.pcapng – The packet capture file containing all recorded traffic.  

README.md – This documentation/report.  

(Optional) Screenshots of Wireshark filters and protocol views.  

Key Concepts Learned  
- Packet capture and filtering.  
- Understanding protocol roles in network communication.  
- Recognizing encrypted vs. unencrypted traffic.  
- Practical use of Wireshark for troubleshooting.
