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

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Subnet Mask
- 11111111.11111111.11111111.10000000 = /25
- 255.255.255.128 = decimal
