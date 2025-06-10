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
`RTA(config)# line vty 0 4 RTA(config-line)# transport input ssh`<br>
`RTA(config-line)# login local`<br>
n. Set the EXEC mode timeout to 6 minutes on the VTY lines.<br>
`RTA(config-line)# exec-timeout 6`<br>
o. Save the configuration to NVRAM.<br>
p. Access the command prompt on the desktop of **PCA** to establish an SSH connection to **RTA**.<br>
`C:\> ssh /?`

