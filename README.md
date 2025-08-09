# Basic Firewall Management

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



