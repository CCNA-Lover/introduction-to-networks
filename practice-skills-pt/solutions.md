# Step 1: Determine the IP Addressing Scheme.

**Bold** entries are data that were missing in the Addressing Table from [Step 1](tasks.md).<br>
*Link-local* address of both interfaces of the Town Hall Router is **FE80::1**. This is also the default gateway for all host (PS: A server is also a host.)

|Device|IPv4 Address|Subnet Mask|IPv6 Address|Default Gateway|
|:---:|:---:|:---:|:---:|:---:|
|TH G0/0|**192.168.1.126**|**255.255.255.224**|2001:DB8:ACAD:A::1/64|-|
|TH G0/1|**192.168.1.158**|**255.255.255.240**|2001:DB8:ACAD:B::1/64|-|
|Administration Switch SVI|**192.168.1.157**|**255.255.255.240**|-|**192.168.1.158**|
|Receptio Host|**192.168.1.97**|**255.255.255.224**|2001:DB8:ACAD:A::FF/64|**192.168.1.126**|
|Operator Host|**192.168.1.98**|**255.255.255.224**|2001:DB8:ACAD:A::15/64|**192.168.1.126**|
|IT Host|**192.168.1.145**|**255.255.255.240**|2001:DB8:ACAD:B::FF/64|**192.168.1.158**|
|Server|**192.168.1.146**|**255.255.255.240**|2001:DB8:ACAD:B::15/64|**192.168.1.158**|

# Step 2: Configure Host Addressing
## Reception Host

![image](https://github.com/user-attachments/assets/5165acf8-801d-4b92-b213-269b0e93ef86)

## Operator Host

![image](https://github.com/user-attachments/assets/e09f7a53-34a9-4978-8e98-3c22123dbc6a)

## IT Host

![image](https://github.com/user-attachments/assets/bf2addd4-abb6-4da2-8ad2-fe92e904302f)

## Server

![image](https://github.com/user-attachments/assets/5d905496-4c3a-40fa-bd82-ca1a47692517)

# Steps 3 & 4: Router & Switch Configurations

## 1. Configuration for Town Hall Router
- Use **line console** to connect **Reception Host** and **Town Hall** router
- Click to **Reception Host** --> **Desktop Tab** --> **Terminal** app --> click **OK**
- Use the configuration script [Town_Hall_router_config.txt](Town_Hall_router_config.txt) as guide to configure the Town Hall Router

## 2. Configuration for Administration Switch
- Using **line console** to connect **IT Host** and **Administration Switch**
- Click to **IT Host** --> **Desktop Tab** --> **Terminal** app --> click **OK**
- Use the configuration script [Administration_Switch_config.txt](Administration_Switch_config.txt) as guide to configure the Administration Switch





