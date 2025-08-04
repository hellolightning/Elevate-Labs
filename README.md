# Local Network Open Port Scan

🎯 Objective:

To discover open ports on devices within the local network using Nmap, and optionally analyze packet captures using Wireshark, in order to understand network exposure and identify potential security risks.


🛠️ Tools Used:

Kali Linux.

Nmap- Free, powerful network scanning tool.

Wireshark-  For capturing and analyzing network traffic.


🔧 Command Used:

ifconfig 

nmap -sS 192.168.232.0/24 -oN scan_results.txt

🔧 Wireshark SYN Packet Filter:
  
Filter used:
tcp.flags.syn == 1 && tcp.flags.ack == 0


🧭 Steps Performed:

Identified the IP of Host device and local IP address range (e.g., 192.168.1.0/24).


![Open Ports](https://github.com/user-attachments/assets/865058a8-7477-4efd-9047-05760ba0b619)

Scanned live hosts with nmap to find open ports.

Saved scan output to a text file and also captured and inspect traffic with Wireshark.


![Nmap Scan Output - Open Ports](https://github.com/user-attachments/assets/9ae95f2b-e8e6-4f1d-b713-7deffdcda624)

![Wireshark SYN Filter](https://github.com/user-attachments/assets/bc32a05f-5a58-49f6-b434-4ea656847965)


🚀 Learning Outcome:

Understood how port scanning works.
Identified running services on devices in the local network.
Practiced ethical network reconnaissance using industry-standard tools.


⚠️ Note:
This project is intended for educational and ethical use only. Do not scan networks or devices without proper authorization.
All scans were performed in a safe, authorized lab environment for educational purposes only
