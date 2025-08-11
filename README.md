# 🛡️ Network Traffic Analysis with Wireshark

This project demonstrates network packet capture and analysis using Wireshark to identify protocols and analyse traffic patterns in a controlled environment.

## Objective:

Capture live network traffic using Wireshark, identify various protocols and traffic and summarize the findings.

## 🛠️ Tools Used

. Wireshark (Free network protocol analyzer)
. Firefox Browser (Traffic generation)
. Target: testphp.vulnweb.com (Vulnerable web application for testing)

## Steps :

1. Install Wireshark

Download wireshark and set up the latest version on Linux.

2. Start Network Capture on Active Interface

Selected my active network interface (wlan0/eth0) in Wireshark.

3. Browse a website or ping a server to generate traffic.

Visited example.com, google.com, and pinged 8.8.8.8.

4. Capture traffic for 1 - 2 Minute

Collected enough packets for analysis.

5. Filtered Packets by Protocol

Applied filters:
                 ``` dns ```
                 ``` tcp ```
                 ``` http ```

6. Identify 3+ Protocols

Observed DNS, TCP, and HTTP.

7. Export Capture File

Save as task5_network_capture.pcap.

8. Analyzed Packets and Summarize your findings and packet details.

Summarized important observations and metadata.


## Protocol Identified:

## Key Findings:


## Key Learning:

. Learned how to capture and analyze real network traffic.

. Successfully identified and analyzed multiple protocols

. Understood the role of DNS, TCP, and HTTP in day-to-day communications.

. Forensic Analysis - Extracted sensitive data from packet captures

. Gained hands-on experience with Wireshark’s filtering and packet inspection tools.


