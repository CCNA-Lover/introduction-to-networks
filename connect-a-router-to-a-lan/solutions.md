# Part 1: Display Router Information

## Step 1: Display interface information on R1.
**Note**: Click a device and then click the **CLI** tab to access the command line directly. The console password is
**cisco**. The privileged EXEC password is **class**.

a. Which command displays the statistics for all interfaces configured on a router?<br>
`R1#show interfaces`<br>
*You have to enter privileged EXEC mode before entering the command*.<br> 
b. Which command displays the information about the Serial 0/0/0 interface only?<br>
`R1#show interfaces s0/0/0`<br>
c. Enter the command to display the statistics for the Serial 0/0/0 interface on R1 and answer the following
questions:<br>
1. What is the IP address configured on **R1**?<br>
**209.165.200.225/30**<br>
2. What is the bandwidth on the Serial 0/0/0 interface?<br>
**1544 kbits**<br><br>

*Snapshot of the output*<br><br>

![sh_int](https://github.com/user-attachments/assets/2cedb318-43a4-4102-85a7-405a89679b75)


d. Enter the command (`R1#show interfaces g0/0`)to display the statistics for the GigabitEthernet 0/0 interface and answer the following
questions:<br>
1. What is the IP address on **R1**?<br>
**There is no IP address configured on the GigabitEthernet 0/0 interface**<br>
2. What is the MAC address of the GigabitEthernet 0/0 interface?<br>
**000d.bd6c.7d01**<br>
3. What is the bandwidth (BW) of the GigabitEthernet 0/0 interface?<br>
**1000000 kbits**<br><br>

*Snapshot of the output*<br><br>

![int_g0](https://github.com/user-attachments/assets/add14b85-0f91-45ad-a1ee-f100edcb40ab)

*bia means **burnt-in address** - other name for the MAC address attributed by the manufacturer; this address is the physical address and is unchangeable*

## Step 2: Display a summary list of the interfaces on R1.
a. Which command displays a brief summary of the current interfaces, interface status, and the IP addresses assigned to them?<br>
`R1#show ip interface brief`<br>
b. Enter the command on each router and answer the following questions:<br><br>

*Interface brief on R1*<br><br>
![ethernet_R1](https://github.com/user-attachments/assets/851d7789-aa81-484b-9ab9-c996deaf0cf0)

*Interface brief on R2*<br><br>
![ethernet_R2](https://github.com/user-attachments/assets/ec102ff9-7f35-4081-a12b-0c394e0e8d1c)


1. How many serial interfaces are there on **R1** and **R2**?<br>
**Each router has 2 serial interfaces**.<br>
2. How many Ethernet interfaces are there on **R1** and **R2**?<br>
**R1 has 6 (2 Gigabit and 4 Fast)Ethernet interfaces and R2 has 2 (Gigabit)Ethernet interfaces**.<br>
3. Are all the Ethernet interfaces on **R1** the same? If no, explain the difference(s).
**No, they are not. There are two Gigabit Ethernet interfaces and 4 Fast Ethernet interfaces. Gigabit Ethernet interfaces support speeds of up to 1,000,000,000 bits per seconds (1 Gbps) and Fast Ethernet interfaces support speeds of up to 1,000,000 bits per second (1 Mbps)**.

## Step 3: Display the routing table on R1.
a. What command displays the contents of the routing table?<br>
`R1#show ip route`<br><br>

*Snapshot of the output*<br><br>
![directly_connected](https://github.com/user-attachments/assets/0a7d7144-fe33-48e3-afbf-67263d91a8a2)

b. Enter the command on **R1** and answer the following questions:<br>
1. How many connected routes are there (uses the **C** code)?<br>
**1**<br>
2. Which route is listed?<br>
**209.165.200.224/30**<br>
3. How does a router handle a packet destined for a network that is not listed in the routing table?<br>
**A router will only send packets to a network listed in the routing table. If a network is not listed, the packet will be dropped.**


# Part 2: Configure Router Interfaces

## Step 1: Configure the GigabitEthernet 0/0 interface on R1.
a. Enter the following commands to address and activate the GigabitEthernet 0/0 interface on **R1**:<br>
`R1(config)# interface gigabitethernet 0/0`<br>
`R1(config-if)# ip address 192.168.10.1 255.255.255.0`<br>
`R1(config-if)# no shutdown`<br>
**Note**: Refer to the [Addressing Table](README.md) to configure the G0/0 interface with the correct IPv4 address.<br>
b. It is good practice to configure a description for each interface to help document the network. Configure an interface description that indicates the device to which it is connected.<br>
`R1(config-if)# description LAN connection to S1`<br>
c. **R1** should now be able to ping PC1.<br>
`R1(config-if)# end`<br>
`R1# ping 192.168.10.10`<br><br>
*Ping successfull to 80% - remaining 20% is due to ARP taking time to resolve the corresponding MAC address of the device with the IP address 192.168.10.10*<br><br>
![R1_ping_successful](https://github.com/user-attachments/assets/200dc80a-a431-4020-b390-ac69c61617f9)

*[R1_config.txt](R1_config.txt) contains all commands to configure the G0/0 interace from Step a to c*

## Step 2: Configure the remaining Gigabit Ethernet Interfaces on R1 and R2.
a. Use the information in the [Addressing Table](README.md) to finish the interface configurations for **R1** and **R2**. For each interface, do the following:<br>
1. Enter the IP address and activate the interface.
2. Configure an appropriate description.<br>
b. Verify interface configurations.<br>
Issue the following commands:<br>
`R1#show ip interface brief`<br>
`R2#show ip interface brief`<br><br>

*Interface brief on R1*<br><br>
![int_br](https://github.com/user-attachments/assets/03496993-51aa-4981-9403-7964c299ab2f)

*Interface brief on R2*<br><br>
![R2_int_br](https://github.com/user-attachments/assets/b9a04916-f286-4242-9f61-7df97fd268b5)

Alternatively issue the following commands to have a more detailed view of the running-config file. Scroll down to verify interface configurations (IP addresses, descriptions, ...):
`R1#show run`<br>
`R2#show run`<br><br>

*Running-config on R1*<br><br>
![R1_sh_run](https://github.com/user-attachments/assets/a28592e3-5278-42dd-bc2c-8e4558d958d8)


*Running-config on R2*<br><br>
![R2_sh_run](https://github.com/user-attachments/assets/c18e9b24-011d-4649-b921-36a73317040c)


*sh ip int br is the short form for show ip interface brief*<br>
**Note**: Refer to the [R1_full_config.txt](R1_full_config.txt) and [R2_full_config.txt](R2_full_config.txt) for Questions 1 and 2.
## Step 3: Back up the configurations to NVRAM.
Save the configuration files on both routers to NVRAM. What command did you use?<br>
**copy run start** (short version of *copy running-config startup-config*).<br>
Include this command in the configuration of the Gigabit Ethernet interfaces for routers R1 and R2 so that changes can be saved to the NVRAM (*Non Volatile RAM*) and uploaded from the *startup-config file* when the router is booted up.

# Part 3: Verify the Configuration

## Step 1: Use verification commands to check your interface configurations.
a. Use the **show ip interface brief** command on both **R1** and **R2** to quickly verify that the interfaces are configured with the correct IP address and are active.<br>
How many interfaces on **R1** and **R2** are configured with IP addresses and in the “up” and “up” state?<br><br>
What part of the interface configuration is NOT displayed in the command output?<br><br>
What commands can you use to verify this part of the configuration?<br><br>
b. Use the **show ip route** command on both **R1** and **R2** to view the current routing tables and answer the following questions:<br>
1. How many connected routes (uses the **C** code) do you see on each router?
2. How many OSPF routes (uses the **O** code) do you see on each router?
3. f the router knows all the routes in the network, then the number of connected routes and dynamically learned routes (OSPF) should equal the total number of LANs and WANs. How many LANs and WANs are in the topology?
4. Does this number match the number of C and O routes shown in the routing table?<br><br>
**Note**: If your answer is "no", thn you are missing a required configuration. Review the steps in Part 2.

## Step 2: Test end-to-end connectivity accross the network.
You should now be able to ping from any PC to any other PC on the network. In addition, you should be able to ping the active interfaces on the routers. For example, the following tests should be successful: 
- From the command line on PC1, ping PC4.
- From the command line on R2, ping PC2.<br>

**Note**: For simplicity in this activity, the switches are not configured. You will not be able to ping them.

