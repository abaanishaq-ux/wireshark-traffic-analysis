# wireshark-traffic-analysis
Task 5 – Wireshark Traffic Capture & Analysis
📌 Objective

The purpose of this task was to capture live network packets using Wireshark and analyze different protocols (HTTP, DNS, TCP). This helps in understanding how data flows through the network and how protocols interact at different layers of the TCP/IP model.

🛠 Tools Used

Wireshark – for packet capturing and analysis

Web Browser – to generate HTTP traffic

Command Prompt (ping) – to generate DNS queries and TCP packets

📂 Steps Performed

Installed Wireshark from the official website.

Started packet capture on the active network interface (Wi-Fi).

Generated traffic by:

Visiting websites in a browser

Using ping google.com in CMD

Stopped capture after ~1 minute.

Applied filters in Wireshark:

http → Showed HTTP requests & responses

dns → Showed DNS queries & responses

tcp → Showed TCP connections & handshakes

Saved capture as .pcap file.

Analyzed protocols and summarized findings.

🔎 Protocols Observed
🌐 HTTP (Hypertext Transfer Protocol)

Application layer protocol used for web browsing.

Works mostly on TCP port 80.

Captured packets showed HTTP GET requests from my system and 200 OK responses from servers.

Since HTTP is unencrypted, full details like requested URLs and headers can be seen.

🔎 DNS (Domain Name System)

Converts domain names (like google.com) into IP addresses.

Uses UDP port 53 for most queries (sometimes TCP for large responses).

Captured packets showed my system sending DNS queries and receiving DNS responses with IP addresses.

Essential for making browsing easier without remembering IP addresses.

🔗 TCP (Transmission Control Protocol)

Transport layer protocol ensuring reliable communication.

Observed the three-way handshake:

SYN → Client initiates connection

SYN-ACK → Server acknowledges

ACK → Client confirms

Provides error-checking, retransmissions, and ordered delivery.

Supports higher-level protocols like HTTP/HTTPS, FTP, SMTP.

📊 Key Learnings

Learned how to capture live network traffic using Wireshark.

Understood how different protocols (HTTP, DNS, TCP) function in real-world communication.

Gained experience in filtering traffic and analyzing packet details (source/destination IP, ports, flags).

Learned importance of packet analysis in network troubleshooting & cybersecurity.

📁 Repository Contents

capture.pcap → The saved Wireshark packet capture file.

README.md → This documentation explaining steps & findings.

✅ Conclusion

This task provided hands-on experience in packet analysis. By capturing live traffic, I could observe how protocols like HTTP, DNS, and TCP interact. Such analysis is crucial in cybersecurity for detecting suspicious activities, troubleshooting network issues, and understanding protocol behavior.
