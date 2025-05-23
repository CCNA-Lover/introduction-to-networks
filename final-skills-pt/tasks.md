# Instructions
In this assessment you will configure the **R1** router and **S1** switch, as you have done in the activities in this course. You will also connect two PCs using a switch and a router that are in the main wiring closet. You will subnet the **192.168.10.0/24** network to provide IPv4 addresses for two subnets that will support the required number of hosts. The larger subnet (LAN 1) requires **100** hosts and the smaller subnet (LAN 2) requires **50** hosts.

# Part 1: Build the Network
a. Build the network according to the logical topology by placing the required equipment in the wiring closet equipment rack.<br>
b. Cable the network devices in the closet as shown in the topology diagram.<br>
c. Connect the hosts as shown in the topology diagram.

# Part 2: Develop an IP Addressing Scheme
In this part of the assessment, you will develop an IP addressing scheme. You will subnet an IPv4 network to create two subnets with the required number of hosts. You will then assign the addresses according to the requirements below. Note that LAN 1 should use the first subnet.<br>

Work with the following information:<br>

- IPv4 Network: **192.168.10.0/24**
- Required number of hosts in IPv4 LAN 1: **100**
- Required number of hosts in IPv4 LAN 2: **50**<br>
Record your subnet assignments according to the following requirements.

1) Assign the first IPv4 address of each subnet to a router interface

- LAN 1 is hosted on **R1 G0/0/1**
- LAN 2 is hosted on **R1 G0/0/0**
3) Assign the last IPv4 address of each subnet to the PC NIC.
4) Assign the second IPv4 address of LAN 1 to **S1** SVI.

# Part 3: Configure Basic Device Settings
Network devices must be configured over a direct console connection. Connectivity between the hosts should be established.

## Step 1: Configure Basic Settings
a. Disable DNS lookup on **R1** and **S1**<br>
b. Configure router hostname using the name **R1**.<br>
c. Configure switch hostname using the name **S1**.<br>
d. Configure an appropriate banner on **R1** and **S1**.<br>
e. Allow console logins with the password **C@nsPassw!**

## Step 2: Configure Interfaces
a. Configure **R1** G0/0/0 and G0/0/1 interfaces using the addressing from the previous part of this assessment:

- Interface description
- IPv4 address / subnet mask<br>
b. Configure the **S1** VLAN 1 SVI interface using the addressing from the previous part of this assessment:

- Interface description
- IPv4 address / subnet mask
- The switch should be reachable from devices on other networks.

# Part 4: Configure Security Settings on R1 and S1
## Step 1: Configure enhanced password security
a. Configure **DontTellAnyone** as the encrypted privileged EXEC password
b. Encrypt all plaintext passwords
c. Set minimum password length to **10** on **R1**.

## Step 2: Configure SSH on R1 and S1
a. Configure **netsec.com** as the domain name<br>
b. Configure a local user netadmin with the secret password **Ci$co12345**<br>
c. Set login on vty lines to use local database.<br>
d. Configure the vty lines to accept SSH access only.<br>
e. Generate an RSA crypto key using 1024 bits modulus.

## Step 3: Secure switch ports on S1
a. Shut down **all** unused ports on **S1**.<br>
b. Enter descriptions for all unused switch ports to indicate that they are intentionally shutdown.

# Part 5: Configure the Hosts and Verify Connectivity
Configure both hosts with the IPv4 addresses that were assigned in Part 2 of this assessment.
