## Step 1: Subnet the 192.168.100.0/24 network into the appropriate number of subnets.
a. Based on the topology, how many subnets are needed?<br><br>
b. How many bits must be borrowed to support the number of subnets in the topology table?<br><br>
c. How many subnets does this create?<br><br>
d. How many usable hosts does this create per subnet?<br><br>
**Note**: If your answer is less than the 25 hosts required, then you borrowed too many bits.<br>
e. Calculate the binary value for the first five subnets. The first two subnets have been done for you.
  | Subnet | Network Address | Bit 7 | Bit 6 | Bit 5 | Bit 4 | Bit 3 | Bit 2 | Bit 1 | Bit 0 |
  |:------:|:--------------:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
  | 0      | 192.168.100.   | 0     | 0     | 0     | 0     | 0     | 0     | 0     | 0     |
  | 1      | 192.168.100.   | 0     | 0     | 1     | 0     | 0     | 0     | 0     | 0     |
  | 2      | 192.168.100.   | 0     | 0     | 0     | 0     | 0     | 0     | 0     | 0     |
  | 3      | 192.168.100.   | 0     | 0     | 0     | 0     | 0     | 0     | 0     | 0     |
  | 4      | 192.168.100.   | 0     | 0     | 0     | 0     | 0     | 0     | 0     | 0     |

f. Calculate the binary and decimal value of the new subnet mask.

<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <td align="center">First Octet</td>
    <td align="center">Second Octet</td>
    <td align="center">Third Octet</td>
    <td align="center">Mask Bit 7</td>
    <td align="center">Mask Bit 6</td>
    <td align="center">Mask Bit 5</td>
    <td align="center">Mask Bit 4</td>
    <td align="center">Mask Bit 3</td>
    <td align="center">Mask Bit 2</td>
    <td align="center">Mask Bit 1</td>
    <td align="center">Mask Bit 0</td>
  </tr>
  <tr>
    <td align="center">11111111</td>
    <td align="center">11111111</td>
    <td align="center">11111111</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td align="center">First Decimal Octet</td>
    <td align="center">Second Decimal Octet</td>
    <td align="center">Third Decimal Octet</td>
    <td colspan="8" align="center" style="background-color: #e6f0ff;">Fourth Decimal Octet</td>
  </tr>
  <tr>
    <td align="center">255.</td>
    <td align="center">255.</td>
    <td align="center">255.</td>
    <td colspan="8"></td>
  </tr>
</table>

g. Fill in the **Subnet Table**, listing the decimal value of all available subnets, the first and last usable host address, and the broadcast address. Repeat until all addresses are listed.<br>
**Note**: You may not need to use all rows.
**Subnet Table**
| Subnet Number| Subnet Address| First Usable Host Address | Last Usable Address | Broadcast Address |
  |:------:|:--------------:|:-----:|:-----:|:-----:|
  | 0      |   |      |      |      |
  | 1      |    |      |      |      |
  | 2      |    |      |      |      | 
  | 3      |    |      |      |      | 
  | 4      |    |      |      |      |
  | 5     |    |      |      |      |
  | 6     |    |      |      |      |
  | 7     |    |      |      |      |
  | 8     |    |      |      |      |
  | 9     |    |      |      |      |
  | 10     |    |      |      |      |

## Step 2: Assign the subnets to the network shown in the topology.
a. Assign Subnet 0 to the LAN connected to the GigabitEthernet 0/0 interface of R1:<br>
b. Assign Subnet 1 to the LAN connected to the GigabitEthernet 0/1 interface of R1:<br>
c. Assign Subnet 2 to the LAN connected to the GigabitEthernet 0/0 interface of R2:<br>
d. Assign Subnet 3 to the LAN connected to the GigabitEthernet 0/1 interface of R2:<br>
e. Assign Subnet 4 to the WAN link between R1 to R2:

## Step 3: Document the addressing scheme.
Fill in the **Addressing Table** using the following guidelines:<br>
a. Assign the first usable IP addresses in each subnet to R1 for the two LAN links and the WAN link.<br>
b. Assign the first usable IP addresses in each subnet to R2 for the LAN links. Assign the last usable IP address for the WAN link.<br>
c. Assign the second usable IP address in the attached subnets to the switches.<br>
d. Assign the last usable IP addresses to the PCs in each subnet.  
