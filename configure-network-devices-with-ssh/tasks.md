# Instructions
## Step 1: Configure Basic Security on the Router
a. Configure IP addressing on **PCA** according to the [Addressing Table](./README.md).<br>
b. Console into RTA from the Terminal on PCA.<br>
c. Configure the hostname as **RTA**.<br>
d. Configure IP addressing on **RTA** and enable the interface.<br>
e. Encrypt all plaintext passwords.<br>
`RTA(config)# service password-encryption`<br>
f. Set the minimum password length to 10.<br>
`RTA(config)# security password min-length 10`<br>
g. Set a strong secret password of your choosing. **Note**: Choose a password that you will remember, or you will need to reset the activity if you are locked out of the device.<br>
h. Disable DNS lookup.<br>
`RTA(config)# no ip domain-lookup`<br>
i. Set the domain name to **CCNA.com** (case-sensitive for scoring in PT).<br>
`RTA(config)# ip domain-name CCNA.com`<br>
j. Create a user of your choosing with a strong encrypted password.<br>
`RTA(config)# username any_user secret any_password`<br>
k. Generate 1024-bit RSA keys.<br>
**Note**: In Packet Tracer, enter the crypto key generate rsa command and press Enter to continue.<br>
`RTA(config)# crypto key generate rsa`<br>
l. Block anyone for three minutes who fails to log in after four attempts within a two-minute period.<br>
`RTA(config)# login block-for 180 attempts 4 within 120`<br>
m. Configure all VTY lines for SSH access and use the local user profiles for authentication.<br>
`RTA(config)# line vty 0 4`<br>
`RTA(config-line)# transport input ssh`
`RTA(config-line)# login local`<br>
n. Set the EXEC mode timeout to 6 minutes on the VTY lines.<br>
`RTA(config-line)# exec-timeout 6`<br>
o. Save the configuration to NVRAM.<br>
p. Access the command prompt on the desktop of **PCA** to establish an SSH connection to **RTA**.<br>
`C:\> ssh /?`

## Step 2: Configure Basic Security on the Switch
Configure switch **SW1** with corresponding security measures. Refer to the configuration steps on the router if you need additional assistance.<br>

a. Click on **SW1** and select the CLI tab. <br>
b. Configure the hostname as **SW1**.<br>
c. Configure IP addressing on SW1 **VLAN1** and enable the interface.<br>
d. Configure the default gateway address.<br>
e. **Note**: On a switch it is a good security practice to disable unused ports. One method of doing this is to simply shut down each port with the **‘shutdown’** command. This would require accessing each port individually. There is a shortcut method for making modifications to several ports at once by using the **interface range** command. On **SW1** all ports except FastEthernet0/1 and GigabitEthernet0/1 can be shutdown with the following command:.<br>
`SW1(config)# interface range F0/2-24, G0/2`<br>
`SW1(config-if-range)# shutdown`<br>
f. Encrpt all plaintext passwords.<br>
g. Set a strong secret password of your choosing.
h. Disable DNS lookup.<br>
`RTA(config)# no ip domain-lookup`<br>
i. Set the domain name to **CCNA.com** (case-sensitive for scoring in PT).<br>
`SW1(config)# ip domain-name CCNA.com`<br>
j. Create a user of your choosing with a strong encrypted password.<br>
`SW1(config)# username any_user secret any_password`<br>
k. Generate 1024-bit RSA keys.<br>
**Note**: In Packet Tracer, enter the crypto key generate rsa command and press Enter to continue.<br>
`SW1(config)# crypto key generate rsa`<br>
l. Configure all VTY lines for SSH access and use the local user profiles for authentication.<br>
`SW1(config)# line vty 0 15`<br>
`SW1(config-line)# transport input ssh`<br>
`SW1(config-line)# login local`<br>
m. Set the EXEC mode timeout to 6 minutes on the VTY lines.<br>
`SW1(config-line)# exec-timeout 6`<br>
n. Save the configuration to NVRAM.

