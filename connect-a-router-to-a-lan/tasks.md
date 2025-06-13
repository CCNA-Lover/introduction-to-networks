# Part 1: Display Router Information

## Step 1: Display interface information on R1.
**Note**: Click a device and then click the **CLI** tab to access the command line directly. The console password is
**cisco**. The privileged EXEC password is **class**.

a. Which command displays the statistics for all interfaces configured on a router?<br><br>
b. Which command displays the information about the Serial 0/0/0 interface only?<br><br>
c. Enter the command to display the statistics for the Serial 0/0/0 interface on R1 and answer the following
questions:<br>
1. What is the IP address configured on **R1**?<br>
2. What is the bandwidth on the Serial 0/0/0 interface?<br>

d. Enter the command to display the statistics for the GigabitEthernet 0/0 interface and answer the following
questions:<br>
1. What is the IP address on **R1**?<br>
2. What is the MAC address of the GigabitEthernet 0/0 interface?<br>
3. What is the bandwidth (BW) of the GigabitEthernet 0/0 interface?

## Step 2: Display a summary list of the interfaces on R1.
a. Which command displays a brief summary of the current interfaces, interface status, and the IP addresses assigned to them?<br><br>
b. Enter the command on each router and answer the following questions:<br>
1. How many serial interfaces are there on **R1** and **R2**?<br>
2. How many Ethernet interfaces are there on **R1** and **R2**?<br>
3. Are all the Ethernet interfaces on **R1** the same? If no, explain the difference(s).

## Step 3: Display the routing table on R1.
a. What command displays the contents of the routing table?<br><br>
b. Enter the command on **R1** and answer the following questions:<br>
1. How many connected routes are there (uses the **C** code)?<br>
2. Which route is listed?<br>
3. How does a router handle a packet destined for a network that is not listed in the routing table?


# Part 2: Configure Router Interfaces

## Step 1: Configure the GigabitEthernet 0/0 interface on R1.
a. Enter the following commands to address and activate the GigabitEthernet 0/0 interface on **R1**:<br>
`R1(config)# interface gigabitethernet 0/0`<br>
`R1(config-if)# ip address 192.168.10.1 255.255.255.0`<br>
`R1(config-if)# no shutdown`<br>
b. It is good practice to configure a description for each interface to help document the network. Configure an interface description that indicates the device to which it is connected.<br>
`R1(config-if)# description LAN connection to S1`<br>
c. **R1** should now be able to ping PC1.<br>
`R1(config-if)# end`<br>
`R1# ping 192.168.10.10`

## Step 2: Configure the remaining Gigabit Ethernet Interfaces on R1 and R2.
a. Use the information in the Addressing Table to finish the interface configurations for **R1** and **R2**. For each interface, do the following:<br>
1. Enter the IP address and activate the interface.
2. Configure an appropriate description.<br>
b. Verify interface configurations.

## Step 3: Back up the configurations to NVRAM.
Save the configuration files on both routers to NVRAM. What command did you use?


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
- From the command line on R2, ping PC2.
**Note**: For simplicity in this activity, the switches are not configured. You will not be able to ping them.
