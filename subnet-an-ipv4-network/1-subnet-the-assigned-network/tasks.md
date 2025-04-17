## Step 1: Create a subnetting scheme that meets the required number of subnets and required number of host addresses.
In this scenario, you are a network technician assigned to install a new network for a customer. You must create multiple subnets out of the **192.168.0.0/24** network address space to meet the following requirements:<br><br>
a. The first subnet is the LAN-A network. You need a minimum of 50 host IP addresses.<br>
b. The second subnet is the LAN-B network. You need a minimum of 40 host IP addresses.<br>
c. You also need at least two additional unused subnets for future network expansion.<br><br>
**Note**: Variable length subnet masks (VLSMs) will not be used. All hte device subnet masks should be the same length.<br>
d. Answer the following questions to help create a subnetting scheme that meets the stated network requirements:<br>
How many host addresses are needed in the largest required subnet?<br><br>
What is the minimum number of subnets required?<br><br>
The network that you are tasked to subnet is 192.168.0.0/24. What is the /24 subnet mask in binary?<br><br>

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

