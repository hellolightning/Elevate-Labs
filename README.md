# Local Network Open Port Scan

🎯 Objective:
To discover open ports on devices within the local network using Nmap, and optionally analyze packet captures using Wireshark, in order to understand network exposure and identify potential security risks.

🛠️ Tools Used
Kali Linux
Nmap- Free, powerful network scanning tool
Wireshark-  For capturing and analyzing network traffic

🔧 Command Used:
ifconfig 192.168.232.132
nmap -sS 192.168.232.0/24 -oN scan_results.txt




- Wireshark SYN Packet Filter
Filter used:

tcp.flags.syn == 1 && tcp.flags.ack == 0

⚠️ Note: All scans were performed in a safe, authorized lab environment for educational purposes only
