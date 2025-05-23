## IPv4 Classes
|Class|Subnet Mask|Prefix|Address Range|Additional notes|
|:---|:---|:---|:---|:---|
|A|255.0.0.0|/8|0.0.0.0 - 127.255.255.255|127.0.0.0 - 127.0.255.255 for loopback<br>10.0.0.0 - 10.255.255.255 private address|
|B|255.255.0.0|/16|128.0.0.0 - 191.255.255.255|169.254.0.0 -169.254.255.255 for APIPA<br>172.16.0.0 - 172.31.255.255 /12 private address<br>192.168.0.0 - 192.168.255.255 private address|
|C|255.255.255.0|/24|192.0.0.0 - 223.255.255.255||
|D|-|-|224.0.0.0 - 240.255.255.255|Experimental|
|E|-|-|240.0.0.0 - 255.255.255.255|Reserved|

## Rule to determine the number of hosts
Given **n** the number of host bits on a network and **N** the number of **usable host addresses**, then **N = 2<sup>n</sup> - 2**.<br>
**Note**: The first and last addresses are reserved for network and broadcast respectively.

## Rule to determine the number of subnets
Given **m** the number of network bits on a network and **M** the number of **usable host addresses**, then **M = 2<sup>m</sup>**.

## Problem 1:
### Given:
|Network Properties|Value|
|:---|:---|
|Host IP Address|192.168.200.139|
|Original Subnet Mask|255.255.255.0 |
|New Subnet Mask|255.255.255.224|

### Find:
|Element|Value|
|:---|:---|
|Number of Subnet Bits|3|
|Number of Subnets Created|8|
|Number of Host Bits per Subnet|5|
|Number of Hosts per Subnet|30|
|Network Address of this Subnet|192.168.200.128|
|IPv4 Address of First Host on this Subnet|192.168.200.129|
|IPv4 Address of Last Host on this Subnet|192.168.200.158|
|IPv4 Broadcast Address on this Subnet|192.168.200.159|

**Explanation:**<br>
192.168.200.139 is a class **C** address with the original prefix of **/24**.<br>
Decimal number in the **fourth octet** of the new subnet mask is **224**.<br>
`224 = 128 + 64 + 32` --> new prefix is **/27** since **3 bits were borrowed** from the host portion **to the network portion**.<br>
Every bit is dual (i.e. has two possible values: *0* or *1*) so there are **2<sup>3</sup> = 8** subnets created<br>
With 5 bits remaining for the host portion, there are **2<sup>5</sup> = 32** addresses, but only **30** are avilable for hosts.

## Problem 2:
### Given:
|Network Properties|Value|
|:---|:---|
|Host IP Address|10.101.99.228|
|Original Subnet Mask|255.0.0.0|
|New Subnet Mask|255.255.128.0|

### Find:
|Element|Value|
|:---|:---|
|Number of Subnet Bits|9|
|Number of Subnets Created|512|
|Number of Host Bits per Subnet|15|
|Number of Hosts per Subnet|32,766|
|Network Address of this Subnet|10.101.0.0|
|IPv4 Address of First Host on this Subnet|10.101.0.1|
|IPv4 Address of Last Host on this Subnet|10.101.127.254|
|IPv4 Broadcast Address on this Subnet|10.101.127.255|

**Explanation:**<br>
10.101.99.228 is a class **A** address with the original prefix of **/8**.<br>
Decimal number in the **second octet** of the new subnet mask is **255**.<br>
`255 = 128 + 64 + ... + 3 + 2 + 1` --> 8 bits borrowed<br>
Decimal number in the **third octet** of the new subnet mask is **128**.<br>
`128 = 128` --> 1 bit borrowed<br>
New prefix is **/17** since **9 bits were borrowed** in total from the host portion **to the network portion**.<br>
Every bit is dual (i.e. has two possible values: *0* or *1*) so there are **2<sup>1</sup> = 2** subnets created<br>
With 15 bits remaining for the host portion, there are **2<sup>15</sup> = 32768** addresses, but only **32766** are avilable for hosts.

## Problem 3:
### Given:
|Network Properties|Value|
|:---|:---|
|Host IP Address|172.22.32.12|
|Original Subnet Mask|255.255.0.0|
|New Subnet Mask|255.255.224.0|

### Find:
|Element|Value|
|:---|:---|
|Number of Subnet Bits|3|
|Number of Subnets Created|8|
|Number of Host Bits per Subnet|13|
|Number of Hosts per Subnet|8190|
|Network Address of this Subnet|172.22.32.0|
|IPv4 Address of First Host on this Subnet|172.22.32.1|
|IPv4 Address of Last Host on this Subnet|172.22.63.254|
|IPv4 Broadcast Address on this Subnet|172.22.63.255|

**Explanation:**<br>
172.22.32.12 is a class **B** address with the original prefix of **/16**.<br>
Decimal number in the **third octet** of the new subnet mask is **224**.<br>
`224 = 128 + 64 + 32` --> new prefix is **/19** since **3 bits were borrowed** from the host portion **to the network portion**.<br>
Every bit is dual (i.e. has two possible values: *0* or *1*) so there are **2<sup>3</sup> = 8** subnets created<br>
With 13 remaining bits for the host portion, there are **2<sup>13</sup> = 8192** addresses, but only **8190** are avilable for hosts.

## Problem 4:
### Given:
|Network Properties|Value|
|:---|:---|
|Host IP Address|192.168.1.245|
|Original Subnet Mask|255.255.255.0|
|New Subnet Mask|255.255.255.252|

### Find:
|Element|Value|
|:---|:---|
|Number of Subnet Bits|6|
|Number of Subnets Created|64|
|Number of Host Bits per Subnet|2|
|Number of Hosts per Subnet|2|
|Network Address of this Subnet|192.168.1.244|
|IPv4 Address of First Host on this Subnet|192.168.1.245|
|IPv4 Address of Last Host on this Subnet|192.168.1.246|
|IPv4 Broadcast Address on this Subnet|192.168.1.247|

**Explanation:**<br>
192.168.1.245 is a class **C** address with the original prefix of **/24**.<br>
Decimal number in the **fourth octet** of the new subnet mask is **252**.<br>
`252 = 128 + 64 + 32 + 16 + 8 + 4` --> new prefix is **/30** since **6 bits were borrowed** from the host portion **to the network portion**.<br>
Every bit is dual (i.e. has two possible values: *0* or *1*) so there are **2<sup>6</sup> = 64** subnets created<br>
With 2 remaining bits for the host portion, there are **2<sup>2</sup> = 4** addresses, but only **2** are avilable for hosts.

## Problem 5:
### Given:
|Network Properties|Value|
|:---|:---|
|Host IP Address|128.107.0.55|
|Original Subnet Mask|255.255.0.0|
|New Subnet Mask|255.255.255.0|

### Find:
|Element|Value|
|:---|:---|
|Number of Subnet Bits|8|
|Number of Subnets Created|256|
|Number of Host Bits per Subnet|8|
|Number of Hosts per Subnet|254|
|Network Address of this Subnet|128.107.0.0|
|IPv4 Address of First Host on this Subnet|128.107.0.1|
|IPv4 Address of Last Host on this Subnet|128.107.0.254|
|IPv4 Broadcast Address on this Subnet|128.107.0.255|

**Explanation:**<br>
128.107.0.55 is a class **B** address with the original prefix of **/16**.<br>
Decimal number in the **third octet** of the new subnet mask is **255**.<br>
`255 = 128 + 64 + 32 + 16 + ... + 2 + 1` --> new prefix is **/24** since **8 bits were borrowed** from the host portion **to the network portion**.<br>
Every bit is dual (i.e. has two possible values: *0* or *1*) so there are **2<sup>8</sup> = 256** subnets created<br>
With 8 remaining bits for the host portion, there are **2<sup>8</sup> = 256** addresses, but only **254** are avilable for hosts.

## Problem 6:
### Given:
|Network Properties|Value|
|:---|:---|
|Host IP Address|192.135.250.180|
|Original Subnet Mask|255.255.255.0|
|New Subnet Mask|255.255.255.248|

### Find:
|Element|Value|
|:---|:---|
|Number of Subnet Bits|5|
|Number of Subnets Created|32|
|Number of Host Bits per Subnet|3|
|Number of Hosts per Subnet|6|
|Network Address of this Subnet|192.135.250.176|
|IPv4 Address of First Host on this Subnet|192.135.250.177|
|IPv4 Address of Last Host on this Subnet|192.135.250.182|
|IPv4 Broadcast Address on this Subnet|192.135.250.183|

**Explanation:**<br>
192.135.250.180 is a class **C** address with the original prefix of **/24**.<br>
Decimal number in the **fourth octet** of the new subnet mask is **248**.<br>
`248 = 128 + 64 + 32 + 16 + 8` --> new prefix is **/29** since **5 bits were borrowed** from the host portion **to the network portion**.<br>
Every bit is dual (i.e. has two possible values: *0* or *1*) so there are **2<sup>5</sup> = 32** subnets created<br>
With 3 remaining bits for the host portion, there are **2<sup>3</sup> = 8** addresses, but only **6** are avilable for hosts.

# Reflection Question
Why is the subnet mask so important when analyzing an IPv4 address?

## Answer
The subnet mask is a variable that divides a an IPv4 address into two separate parts: the network and the host portion. Advantages are:
1. **efficient routing** - routers forward packets based on network identification (the network portion determined by the subnet mask)
2. **branch-specific IPv4 address allocation** - more manageable subnets are created based on the requirements of each and every nerwork (security, physical location, department, etc.)
3. **broadcast domain control** - broadcast traffic is limited to specific network segments (portions)
4. **route aggregation** - subnet masks facilitate route summarization (supranetting)
