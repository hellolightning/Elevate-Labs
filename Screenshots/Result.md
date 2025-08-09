# Testing the Firewall Rules on Linux

To verify UFW’s filtering:

Block inbound traffic on port 23 (Telnet):  ``` sudo ufw deny 23/tcp ```

![3 Set Default policy](https://github.com/user-attachments/assets/2114b001-c3d7-469f-b1f1-5f9f908632a8)

Attempt to connect to port 23 remotely using: ``` telnet 23 ``` OR 

Use other system to test with following command: ``` nmap -p 23 your_ip ```

![4 Test firewall rules](https://github.com/user-attachments/assets/76ea2065-37d8-425c-aceb-b545db0815d4)

The connection failed, confirming that port 23 was successfully blocked.

Allow SSH access on port 22: ``` sudo ufw allow 22/tcp ```

Remove the block on port 23 to restore normal access: ``` List numbered rules: ``` , ``` sudo ufw status numbered ```

Delete the deny rule blocking port 23 by its rule number (for example, if rule number is 3): ``` sudo ufw delete 3 ```


### This testing demonstrated that UFW effectively enforces firewall policies, controlling network access and enhancing Linux system security
