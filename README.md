# 🛡️ Basic Firewall Management

This repository provides a report of comprehensive analysis of the UFW (Uncomplicated Firewall) setup and configuration performed on a Kali Linux system, demonstrating practical network security implementation and testing.

## Objective: 

Configure and test basic firewall rules using UFW to control network traffic flow

System: Kali Linux (192.168.37.130)

## Step-by-step Process:

1. Open firewall configuration:
   
    Linux (UFW): ``` sudo ufw status ```
   
3. Installing UFW in linux : ``` sudo apt update && sudo apt install ufw ```

![1 Install UFW](https://github.com/user-attachments/assets/4a97a449-d01d-41d5-b4af-e5771bd42f45)

2. Enabling UFW : ``` sudo ufw enable ```

![2 Enabling UFW](https://github.com/user-attachments/assets/6398295c-828b-4ffc-bca0-c62d69883aee)

3. Make UFW start on boot : ``` sudo systemctl enable ufw ```

4. Enable logging to monitor firewall activity : ``` sudo ufw logging on ```

5. Set Default policy in UFW : ``` sudo ufw default deny incoming sudo ufw default allow outgoing ```
   
6. Block a specific port ( Block Inbound Traffic on Port 23 (Telnet) ) : ``` sudo ufw deny 23/tcp sudo ufw deny 23/udp ```

7. Allow SSH Access (Port 22) : ``` sudo ufw allow ssh ```
   
![3 Set Default policy](https://github.com/user-attachments/assets/d1841af7-3c88-48da-9f9b-97e7da5d7234)

8. Test firewall rules.
   
9. Remove the test block rule to restore original state.
 
## End Result

![5 End Result](https://github.com/user-attachments/assets/c62738ce-4e84-475e-a5f7-1c611728d96a)

## Security Impact Assessment 

### Threat Mitigation Achieved:

Default-deny incoming policy blocks unsolicited inbound traffic, reducing the attack surface.

Denying Telnet (port 23) prevents exploitation of this insecure, outdated protocol.

Allow-listing SSH ensures only necessary remote access is permitted while other services remain blocked.

### Operational Considerations: 

Controlled traffic flow—only necessary services permitted, simplifying monitoring and auditing.

Improved visibility via logging—with ufw logging on, administrators can monitor, detect and respond to anomalies activity effectively.

Automatic startup on boot—using systemctl enable ufw, ensures firewall protection always boots up, improving consistency.

## Best Practices Demonstrated 

### Configuration Management:

Explicit default policies defined—‘deny incoming’ and ‘allow outgoing’ establish a clear baseline.

Managed rule additions/removals—the flow includes both applying and later removing test rules, showing responsible rule lifecycle.

### Security Principles Applied:

Principle of least privilege—only essential ports (SSH) are allowed, everything else is denied by default.

Defense in depth—UFW adds a layer of protection even if other services lack hardening.

## Technical Deep Dive 

### UFW Architecture Understanding: 

UFW operates as a frontend to iptables, providing simplified rule management while maintaining the robust filtering capabilities of the underlying netfilter framework. UFW is a simplified, user-friendly frontend to manage firewall rules on Kali Linux, designed for basic firewall control and protection.
The implementation demonstrates:

- Rule configuration – You define firewall behavior by setting default rules (e.g., deny incoming, allow outgoing), then add targeted rules such as denying specific ports (e.g., Telnet port 23) and allowing services like SSH (port 22).

- Persistence & Startup: UFW can be enabled to start automatically on boot (e.g., 1``sudo systemctl enable ufw``), ensuring firewall rules remain active after restarts.

- Monitoring and testing – UFW allows logging of firewall activity, letting you observe how traffic is being handled, and you can test rules to confirm they're working, then fine-tune or remove test rules based on results.

  
