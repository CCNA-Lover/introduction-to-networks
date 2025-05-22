# Step 1: Determine the IP Addressing Scheme.
Design an IPv4 addressing scheme and complete the Addressing Table based on the following requirements.

a. Subnet the 192.168.1.0/24 network to provide 30 host addresses per subnet while wasting the fewest addresses.<br>
b. Assign the fourth subnet to the **IT Department LAN**.<br>
c. Assign the last network host address (the highest) in this subnet to the G0/0 interface on **Town Hall**.<br>
d. Starting with the fifth subnet, subnet the network again so that the new subnets will provide 14 host addresses per subnet while wasting the fewest addresses. <br>
e. Assign the second of these new 14-host subnets to the Administration LAN.<br> 
f. Assign the last network host address (the highest) in the **Administration LAN** subnet to the G0/1 interface of the **Town Hall** router.<br>
g. Assign the second to the last address (the second highest) in this subnet to the VLAN 1 interface of the **Administration Switch**.<br>
h. Configure addresses on the hosts using any of the remaining addresses in their respective subnets.<br>

# Step 2: Configure Host Addressing
a. Use the IPv4 addressing from Step 1 and the IPv6 addressing values provided in the Addressing Table to configure all host PCs with the correct addressing.<br>
b. Use the router interface link-local address as the IPv6 default gateways on the hosts.<br>
c. Complete the configuration of the server using the IPv4 addressing values from Step 1 and the values in the addressing table<br>

# Step 3: Configure the Town Hall Router.
a. Configure the **Town Hall** router with all initial configurations that you have learned in the course so far:

- Configure the router hostname: **CS-Department**
- Protect device configurations from unauthorized access with the encrypted privileged exec password.
- Secure all access lines into the router using methods covered in the course and labs.
- Require newly-entered passwords to have a minimum length of 10 characters.
- Prevent all passwords from being viewed in clear text in device configuration files.
- Configure the router to only accept in-band management connections over the protocol that is more secure than Telnet, as was done in the labs and PT activities. Use the value **1024** for encryption key strength.
- Configure local user authentication for in-band management connections. Create a user with the name **netadmin** and a secret password of **Cisco_CCNA7**.<br>

b. Configure the two Gigabit Ethernet interfaces using the IPv4 addressing values that you calculated and the IPv6 values provided in the addressing table.

- Reconfigure the link local addresses to the value shown in the table.
- Document the interfaces in the configuration file.
  
# Step 4: Configure the Administration Switch.
**Configure Administration Switch for remote management over Telnet.**

a. Configure VLAN 1 as the SVI.<br>
b. Configure IPv4 addressing according to your work in Step 1.<br>
c. Be sure that the switch is able to accept connections from hosts on other networks.
