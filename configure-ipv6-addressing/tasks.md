# Part 1: Configure IPv6 Addressing on the Router 
## Step 1: Enable the router to forward IPv6 packets. 
a. Click **R1** and then the **CLI**. Press **Enter**.<br>
b. Enter privileged EXEC mode.<br>
c. Enter the **ipv6 unicast-routing** global configuration command. This command must be entered to enable the router to forward IPv6 packets.<br>
`R1(config)# ipv6 unicast-routing`
## Step 2: Configure IPv6 addressing on GigabitEthernet0/0.
a. Enter the commands necessary to move to interface configuration mode for GigabitEthernet0/0.<br>
b. Configure the IPv6 address with the following command: <br>
`R1(config-if)# ipv6 address 2001:db8:1:1::1/64`<br>
c. Configure the link-local IPv6 address with the following command:<br>
`R1(config-if)# ipv6 address fe80::1 link-local`<br>
d. Activate the interface.<br>
`R1(config-if)# no shutdown`
## Step 3: Configure IPv6 addressing on GigabitEthernet0/1.
a. Enter the commands necessary to move to interface configuration mode for GigabitEthernet0/1.<br>
b. Refer to the Addressing Table for the correct IPv6 address.<br>
c. Configure the IPv6 address, the link-local address and activate the interface.
## Step 4: Configure IPv6 addressing on Serial0/0/0.
a. Enter the commands necessary to move to interface configuration mode for Serial0/0/0.<br>
b. Refer to the Addressing Table for the correct IPv6 address.<br>
c. Configure the IPv6 address, the link-local address and activate the interface.
## Step 5: Verify IPv6 addressing on R1. It is good practice to verify addressing when it is complete by comparing configured values with the values in the addressing table.
a. Exit configuration mode on R1.<br>
b. Verify the addressing configured by issuing the following command:<br>
`R1# show ipv6 interface brief`<br>
c. If any addresses are incorrect, repeat the steps above as necessary to make any corrections.<br>
Note: To make a change in addressing with IPv6, you must remove the incorrect address or else both the correct address and incorrect address will remain configured on the interface.<br>
Example:
`R1(config-if)# no ipv6 address 2001:db8:1:5::1/64`<br>
d. Save the router configuration to NVRAM.
