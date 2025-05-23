# Part 1: Build the Network
**Follow these steps to complete Part 1 of the Final Skills Exam.** <br>
- Placing Switch S1 and Router R1 to wiring closet equipment rack.
- Using **Copper Straight-Through** cable to connect **PC-A** (FastEthernet0 port) and **S1** (FastEthernet0/6 port)
- Same as above, using **Copper Straight-Through** cable to connect all devices as shown in the topology diagram.
- **Turn-on PCs and Router R1**

# Part 2: Develop an IP Addressing Scheme

|Item|Requirements|IPv4 Address|Subnet Mask|
|:---:|:---:|:---:|:---:|
|Network Address|192.168.10.0/24|||
|LAN 1 subnet host requirements|100|**192.168.10.0/25**|**255.255.255.128**|
|LAN 2 subnet host requirements|50|**192.168.10.128/26**|**255.255.255.192**|
|R1 G0/0/1|First host address in LAN 1 subnet|**192.168.10.1/25**|**255.255.255.128**|
|R1 G0/0/0|First host address in LAN 2 subnet|**192.168.10.129**||
|S1 SVI|Second host address in LAN 1 subnet|**192.168.10.2**||
|PC-A|Last host address in LAN 1 subnet|**192.168.10.126**||
|PC-B|Last host address in LAN 2 subnet|**192.168.10.190**||

# Parts 3 & 4: Basic Device and Security Configurations
## 1. Configuration for Router R1
- Using **line console** to connect PC-A and Router
- Click to **PC-A** --> **Terminal** app --> click **OK**
- Use the configuration script **R1_config.txt** as guide to configure the Router R1

## 2. Configuration for Switch S1
- Using **line console** to connect PC-B and Switch
- To show Console port on Switch, **Right click** Switch --> **Inspect Rear** --> **Console port**
- Use the configuration script [**S1_config.txt**](S1_config.txt) as guide to configure the Switch S1

# Part 5: Configure the Hosts and Verify Connectivity
On PCs, go to **Desktop** tab --> **IP Configuration** menu
## PC-A
![image](https://github.com/user-attachments/assets/dee518b4-5086-4c19-acb1-b11d2f64eac3)
## PC-B
![image](https://github.com/user-attachments/assets/032d4520-d465-479e-b761-df3479436bd1)

|Hosts|IPv4 Address|Subnet Mask|IPv4 Default Gateway|
|:---:|:---:|:---:|:---:|
|PC-A|**192.168.10.126**|**255.255.255.128**|**192.168.10.1**|
|PC-B|**192.168.10.190**|**255.255.255.192**|**192.168.10.129**|




