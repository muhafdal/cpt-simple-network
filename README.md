# Simple Network
Design a network in Cisco Packet Tracer to connect ACCOUNTS and DELIVERY departments through the following:
- Each department should contain at least two PCs.
- An appropriate number of switches and routers should be used in the network.
- Using the given network 192.168.40.0, all interfaces sould be configured with correct IP addresses, subnet mask and gateways.
- All devices in the network should be connected using appropriate cables.
- Test communication between devices in both ACCOUNTS and DELIVERY departments.
  
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

- Network Address:192.168.40.0
- Subnets needed:2
  
# Number of Subnets:
- 2^x = Subnets needed
- 2^x = 2
- x = 2/2
- x = 1, we have 1 as the number of ones in the last octet

# Subnet Mask:
- 11111111.11111111.11111111.10000000 = /25
- 255.255.255.128 = decimal

# Number of Hosts:
- 2^y-2 = Number of Hosts (y is the number of zeros in the last octet)
- 2^7-2 = (Subtract 2 for IP network and broadcast network)
- 128-2 = 126

# Subnet Block:
- 256-last decimal of subnet mask = Subnet Block
- 256-128 = 128


- Subnet Number = 0, 128 

# 1st Subnet
- Subnet Mask: 255.255.255.128
- Network Address: 192.168.40.0
- Min: 192.168.40.1 (network +1)
- Max: 192.168.40.126 (broadcast -1)
- Broadcast Address: 192.168.40.127 (0–127 range = 128 addresses)
# 2nd Subnet
- Subnet Mask: 255.255.255.128
- Network Address: 192.168.40.128 (previous subnet’s broadcast +1)
- Min: 192.168.40.129 (network +1)
- Max: 192.168.40.254 (broadcast -1)
- Broadcast Address: 192.168.40.255 (128–255 range = 128 addresses)



