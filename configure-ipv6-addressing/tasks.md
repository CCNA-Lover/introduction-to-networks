
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
Example:<br>
`R1(config-if)# no ipv6 address 2001:db8:1:5::1/64`<br>
d. Save the router configuration to NVRAM.


# Part 2:  Configure IPv6 Addressing on the Servers


## Step 1: Configure IPv6 addressing on the Accounting Server.
a. Click **Accounting** and click the **Desktop** tab > **IP Configuration**.<br>
b. Set the **IPv6 Address** to **2001:db8:1:1::4** with a prefix of **/64**.<br>
c. Set the **IPv6 Gateway** to the link-local address, **fe80::1**.

## Step 2: Configure IPv6 addressing on the CAD Server.
Configure the **CAD** server with addresses as was done in Step 1. Refer to the **Addressing Table** for the addresses to use.


# Part 3: Configure IPv6 Addressing on the Clients

## Step 1: Configure IPv6 addressing on the Sales and Billing Clients.
a. Click **Billing** and then select the **Desktop** tab followed by **IP Configuration**.<br>
b. Set the **IPv6 Address** to **2001:db8:1:1::3** with a prefix of **/64**.<br>
c. Set the **IPv6 Gateway** to the link-local address, **fe80::1**.<br>
d. Repeat Steps 1a through 1c for **Sales**. Refer to the **Addressing Table** for the IPv6 address.

## Step 2: Configure IPv6 Addressing on the Engineering and Design Clients.
a. Click **Engineering** and then select the **Desktop** tab followed by **IP Configuration**.<br>
b. Set the IPv6 Address to **2001:db8:1:2::3** with a prefix of **/64**.<br>
c. Set the **IPv6 Gateway** to the link-local address, **fe80::1**.<br>
d. Repeat Steps 2a through 2c for **Design**. Refer to the **Addressing Table** for the IPv6 address.


# Part 4: Test and Verify Network Connectivity

## Step 1: Open the server web pages from the clients.
a. Click **Sales** and click the **Desktop** tab. Close the **IP Configuration** window, if necessary.<br>
b. Click **Web Browser**. Enter **2001:db8:1:1::4** in the URL box and click **Go**. The **Accounting** website should appear.<br>
c. Enter **2001:db8:1:2::4** in the URL box and click **Go**. The **CAD** website should appear.<br>
d. Repeat steps 1a through 1c for the rest of the clients.

## Step 2: Ping the ISP.
a. Click on any client.<br>
b. Click the Desktop tab > Command Prompt.<br>
c. Test connectivity to the ISP by entering the following command:<br>
`PC> ping 2001:db8:1:a001::1`<br>
d. Repeat the **ping** command with other clients until full connectivity is verified.

