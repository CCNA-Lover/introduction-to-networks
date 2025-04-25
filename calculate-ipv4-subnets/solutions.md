**Recall: IPv4 Address Classes:**<br>
|Class|Subnet Mask|Prefix|Address Range|Additional notes|
|:---|:---|:---|:---|:---|
|A|255.0.0.0|/8|0.0.0.0 - 127.255.255.255||
|B|255.255.0.0|/16|128.0.0.0 - 191.255.255.255||
|C|255.255.255.0|/24|192.0.0.0 - 223.255.255.255||
|D|N/A|N/A|224.0.0.0 - 240.255.255.255|Experimental|
|E|N/A|N/A|240.0.0.0 - 255.255.255.255|Reserved|

## Problem 1:
### Given:
|Network Properties|Value|
|:---|:---|
|Host IP Address|192.168.200.139 |
|Original Subnet Mask|255.255.255.0 |
|New Subnet Mask|255.255.255.224|

### Find:
|Element|Value|
|:---|:---|
|Number of Subnet Bits|3|
|Number of Subnets Created|8|
|Number of Host Bits per Subnet|5|
|Number of Hosts per Subnet|30|
|Network Address of this Subnet||
|IPv4 Address of First Host on this Subnet|192.168.200.129|
|IPv4 Address of Last Host on this Subnet|192.168.200.158|
|IPv4 Broadcast Address on this Subnet|192.168.200.159|

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
|IPv4 Address of First Host on this Subnet|10.101.1.0|
|IPv4 Address of Last Host on this Subnet|10.101.126.0|
|IPv4 Broadcast Address on this Subnet|10.101.127.0|

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
|IPv4 Address of Last Host on this Subnet|172.22.62.0|
|IPv4 Broadcast Address on this Subnet|172.22.63.0|

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

# Reflection Question
Why is the subnet mask so important when analyzing an IPv4 address?
