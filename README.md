# Simple Network
## Version: 8.2.2
### Design a network in Cisco Packet Tracer to connect ACCOUNTS and DELIVERY departments through the following:
- Each department should contain at least two PCs.
- An appropriate number of switches and routers should be used in the network.
- Using the given network 192.168.40.0, all interfaces sould be configured with correct IP addresses, subnet mask and gateways.
- All devices in the network should be connected using appropriate cables.
- Test communication between devices in both ACCOUNTS and DELIVERY departments.
  
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Network Address: 192.168.40.0  
Subnets needed: 2  
  
### Number of Subnets:
- 2^x = Subnets needed
- 2^x = 2
- 2^1 = 2
- x = 1, we have 1 as the number of ones in the last octet

### Subnet Mask:
- 11111111.11111111.11111111.10000000 = /25
- 255.255.255.128 = decimal

### Number of Hosts:
- 2^y-2 = Number of Hosts (y is the number of zeros in the last octet)
- 2^7-2 = (Subtract 2 for IP network and broadcast network)
- 128-2 = 126

### Subnet Block:
- 256-last decimal of subnet mask = Subnet Block
- 256-128 = 128
- Subnet Number = 0, 128 

### 1st Subnet
- Subnet Mask: 255.255.255.128
- Network Address: 192.168.40.0
- Min: 192.168.40.1 (network +1)
- Max: 192.168.40.126 (broadcast -1)
- Broadcast Address: 192.168.40.127 (0–127 range = 128 addresses)
### 2nd Subnet
- Subnet Mask: 255.255.255.128
- Network Address: 192.168.40.128 (previous subnet’s broadcast +1)
- Min: 192.168.40.129 (network +1)
- Max: 192.168.40.254 (broadcast -1)
- Broadcast Address: 192.168.40.255 (128–255 range = 128 addresses)  

### Enable interfaces Gig0/0 and Gig0/1
![1](https://github.com/user-attachments/assets/98328e25-eb02-4b4a-824d-4026cbf7221a)  
![2](https://github.com/user-attachments/assets/0e7ad96c-e183-4310-aba1-7452b519c3a1)  
![3](https://github.com/user-attachments/assets/2cf1a999-0248-41d9-9167-7758659807ea)  
### Set IP address
#### Router
![4](https://github.com/user-attachments/assets/a1fe289b-933c-4b5e-a7d6-63b3706baccc)  
In order to view the assigned IP, use the command:
```
do show start
```
![5](https://github.com/user-attachments/assets/261df3f3-7bbb-47ef-bac4-087a5c155c67)  
#### PC in the Accounts Department
![6](https://github.com/user-attachments/assets/8674fceb-6cc1-4c0b-ab47-74594703c407)  
#### Printer in the Accounts Department
![7](https://github.com/user-attachments/assets/1c6da9b9-85eb-4cfd-9eec-73d2d34345c1) 
![8](https://github.com/user-attachments/assets/4641c1df-2430-4db8-9ee4-95cb39f55de7)  
#### PC in the Delivery Department
![9](https://github.com/user-attachments/assets/a06a3162-b84a-46f9-8457-6117069b16fe)  
#### Printer in the Delivery Department
![10](https://github.com/user-attachments/assets/dd402d95-3663-47e9-8a96-bb8c79b8559f)  
![11](https://github.com/user-attachments/assets/4b2a910d-feb1-4978-81cc-5cf31cc84344)  
### Check the Connection
#### Perform a ping test from the Accounts Department PC to the Delivery Department PC and printer
![12](https://github.com/user-attachments/assets/eed0eeb7-2157-48a5-8f00-bc5be2120430)  
#### Perform a ping test from the Delivery Department PC to the Accounts Department PC and printer
![13](https://github.com/user-attachments/assets/ebb4b5a9-e273-4061-a81c-df12399fe02e)  
