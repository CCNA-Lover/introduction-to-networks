## Step 1: Create a subnetting scheme that meets the required number of subnets and required number of host addresses.
In this scenario, you are a network technician assigned to install a new network for a customer. You must create multiple subnets out of the **192.168.0.0/24** network address space to meet the following requirements:<br><br>
a. The first subnet is the LAN-A network. You need a minimum of 50 host IP addresses.<br>
b. The second subnet is the LAN-B network. You need a minimum of 40 host IP addresses.<br>
c. You also need at least two additional unused subnets for future network expansion.<br>
**Note**: Variable length subnet masks (VLSMs) will not be used. All hte device subnet masks should be the same length.<br>
d. Answer the following questions to help create a subnetting scheme that meets the stated network requirements:<br>
How many host addresses are needed in the largest required subnet?<br><br>
What is the minimum number of subnets required?<br><br>
The network that you are tasked to subnet is 192.168.0.0/24. What is the /24 subnet mask in binary?<br><br>
e. The subnet mask is made up of two portions, the network portion, and the host portion. This is represented in the binary by the ones and the zeros in the subnet mask.<br>
In the network mask, what do the ones represent?<br><br>
In the network mask, what do the zeros represent?<br><br>
f. To subnet a network, bits from the host portion of the original network mask are changed into subnet bits. The number of subnet bits defines the number of subnets.<br><br>
Given each of the possible subnet masks depicted in the following binary format, how many subnets and how many hosts are created in each example?<br><br>
**Hint**: Remember that the number of host bits (to the power of 2) defines the number of hosts per subnet (minus 2), and the number of subnet bits (to the power of two) defines the number of subnets. The subnet bits (shown in bold) are the bits that have been borrowed beyond the original network mask of /24. The /24 is the prefix notation and corresponds to a dotted decimal mask of 255.255.255.0.<br><br>
The network that you are tasked to subnet is 192.168.0.0/24. What is the /24 subnet mask in binary?<br><br>
1. (/25) 11111111.11111111.11111111.**1**0000000<br>
Dotted decimal subnet mask equivalent:<br><br>
Number of subnets? Number of hosts?<br><br>
2. (/26) 11111111.11111111.11111111.**11**000000<br>
Dotted decimal subnet mask equivalent:<br><br>
Number of subnets? Number of hosts?<br><br>
3. (/27) 11111111.11111111.11111111.**111**00000<br>
Dotted decimal subnet mask equivalent:<br><br>
Number of subnets? Number of hosts?<br><br>
4. (/28) 11111111.11111111.11111111.**1111**0000<br>
Dotted decimal subnet mask equivalent:<br><br>
Number of subnets? Number of hosts?<br><br>
5. (/29) 11111111.11111111.11111111.**11111**000<br>
Dotted decimal subnet mask equivalent:<br><br>
Number of subnets? Number of hosts?<br><br>
6. (/30) 11111111.11111111.11111111.**111111**00<br>
Dotted decimal subnet mask equivalent:<br><br>
Number of subnets? Number of hosts?<br><br>
Considering your answers above, which subnet masks meet the required number of minimum host addresses?<br><br>
Considering your answers above, which subnet masks meet the minimum number of subnets required?<br><br>
Considering your answers above, which subnet mask meets both the required minimum number od hosts and the minimum number of subnets required?<br><br>
When you have determined which subnet mask meets all of the stated network requirements, derive each of the subnets. List the subnets from first to last in the table. Remember that the first subnet is 192.168.0.0 with the chosen subnet mask.

| Subnet Address | Prefix | Subnet Mask |
|----------------|--------|-------------|
|                |        |             |
|                |        |             |
|                |        |             |
|                |        |             |
## Step 2: Fill in the missing IP addresses in the Addressing Table.
Assign IP addresses based on the following criteria: Use the ISP Network settings as an example.<br><br>
a. Assign the forst subnet to LAN-A.
1. Use the first host address for the CustomerRouter interface connected to LAN-A switch.
2. Use the second host address for the LAN-A switch. Make sure to assign a default gateway address for the switch.
3. Use the last host address for PC-A. Make sure to assign a default gateway address for the PC.

b. Assign the second subnet to LAN-B.
1. Use the first host address for the CustomerRouter interface connected to LAN-B switch.
2. Use the second host address for the LAN-B switch. Make sure to assign a default gateway address for the switch.
3. Use the last host address for PC-B. Make sure to assign a default gateway address for the PC.

| Device | Interface | IP Address | Subnet Mask | Default Gateway |
|--------|-----------|------------|-------------|-----------------|
| CustomerRouter | G0/0 | | | N/A |
| | G0/1 | | | |
| | S0/1/0 | 209.165.201.2 | 255.255.255.252 | |
| LAN-A Switch | VLAN1 | | | |
| LAN-B Switch | VLAN1 | | | |
| PC-A | NIC | | | |
| PC-B | NIC | | | |
| ISPRouter | G0/0 | 209.165.200.225 | 255.255.255.224 | N/A |
| | S0/1/0 | 209.165.201.1 | 255.255.255.252 | |
| ISPSwitch | VLAN1 | 209.165.200.226 | 255.255.255.224 | 209.165.200.225 |
| ISP Workstation | NIC | 209.165.200.235 | 255.255.255.224 | 209.165.200.225 |
| ISP Server | NIC | 209.165.200.240 | 255.255.255.224 | 209.165.200.225 |
