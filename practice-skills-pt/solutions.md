# Step 1: Determine the IP Addressing Scheme.

Bold entries are data that were missing in the Addressing Table from [Step 1](tasks.md).<br>
*Link-local* address of both interfaces of the Town Hall Router is **FE80::1**. This is also the default gateway for all hosts and the server.

|Device|IPv4 Address|Subnet Mask|IPv6 Address|Default Gateway|
|:---:|:---:|:---:|:---:|:---:|
|TH G0/0|**192.168.1.126**|**255.255.255.224**|2001:DB8:ACAD:A::1/64||
|TH G0/1|**192.168.1.158**|**255.255.255.240**|2001:DB8:ACAD:B::1/64||
|Administration Switch SVI|**192.168.1.157**|**255.255.255.240**||**192.168.1.158**|
|Receptio Host|**192.168.1.97**|**255.255.255.224**|2001:DB8:ACAD:A::FF/64|**192.168.1.126**|
|Operator Host|**192.168.1.98**|**255.255.255.224**|2001:DB8:ACAD:A::15/64|**192.168.1.126**|
|IT Host|**192.168.1.145**|**255.255.255.240**|2001:DB8:ACAD:B::FF/64|**192.168.1.158**|
|Server|**192.168.1.146**|**255.255.255.240**|2001:DB8:ACAD:B::15/64|**192.168.1.158**|




