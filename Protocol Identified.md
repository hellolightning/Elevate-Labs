# Protocols Identified Results

Analyzed captured network traffic using Wireshark and identified different network protocols.

#### 1. HTTP (Hypertext Transfer Protocol) : Application layer protocol for transferring web pages and data between browsers and web servers.

![HTTP](https://github.com/user-attachments/assets/ccd7ab76-feb5-45f8-8bc2-6340344d51b9)

. Packets Analyzed: 162 HTTP requests/responses

. Target Server: testphp.vulnweb.com (44.228.249.3)

. Request Types: POST and GET requests

. Critical Finding: Unencrypted sensitive data transmission


#### 2. DNS (Domain Name System) : System that translates human-readable domain names (like google.com) into IP addresses that computers use.

![DNS](https://github.com/user-attachments/assets/6034410a-62b7-486c-8f37-c04c3dc6ad2c)

. Packets Analyzed: 474 DNS queries/responses

. Primary Queries: youtube.com, testphp.vulnweb.com, acunetix.com

. DNS Server: 192.168.232.132

. Average Response Time: 0.0070 sec


#### 3. TCP (Transmission Control Protocol) : Reliable transport protocol that ensures data is delivered completely and in the correct order between devices.

![TCP](https://github.com/user-attachments/assets/1d4ad941-f492-4ab0-8ef6-c8ddea60fe44)

. Packets Analyzed: 9792 packets displayed

. Purpose: Reliable, connection-oriented transport protocol

. Key Features:
              Three-way handshake connection establishment
              Sequence numbers for ordered delivery


#### 4. ARP (Address Resolution Protocol) : Protocol that maps IP addresses to physical MAC addresses on local network segments.

![ARP](https://github.com/user-attachments/assets/02732088-f7bb-4e04-8c60-db01ca12ec1e)

. Packets Analyzed: 53 ARP requests/responses

. Function: MAC address resolution and network discovery

. Environment: VMware virtual network


