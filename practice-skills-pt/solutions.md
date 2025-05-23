# Step 1: Determine the IP Addressing Scheme.

| Device               | Interface | IP Address/Mask                                                                 | Default Gateway |
|----------------------|-----------|----------------------------------------------------------------------------------|------------------|
| Town Hall            | G0/0      | <font color="red">192.168.1.126/27</font><br><font color="red">(SM: 255.255.255.224)</font><br>2001:db8:acad:a::1/64<br>fe80::1   | N/A              |
|                      | G0/1      | <font color="red">192.168.1.158/28</font><br><font color="red">(SM: 255.255.255.240)</font><br>2001:db8:acad:b::1/64<br>fe80::1   | N/A              |
| Administration Switch| SVI       | <font color="red">192.168.1.157/28</font><br><font color="red">(SM: 255.255.255.240)</font>                                       | <font color="red">192.168.1.158</font>    |
| Reception Host       | NIC       | <font color="red">192.168.1.97/27</font><br><font color="red">(SM: 255.255.255.224)</font><br>2001:db8:acad:a::ff/64             | <font color="red">192.168.1.126</font><br><font color="red">FE80::1</font> |
| Operator Host        | NIC       | <font color="red">192.168.1.98/27</font><br><font color="red">(SM: 255.255.255.224)</font><br>2001:db8:acad:a::15/64             | <font color="red">192.168.1.126</font><br><font color="red">FE80::1</font> |
| IT Host              | NIC       | <font color="red">192.168.1.145/28</font><br><font color="red">(SM: 255.255.255.240)</font><br>2001:db8:acad:b::ff/64            | <font color="red">192.168.1.158</font><br><font color="red">FE80::1</font> |
| Server               | NIC       | <font color="red">192.168.1.146/28</font><br><font color="red">(SM: 255.255.255.240)</font><br>2001:db8:acad:b::15/64            | <font color="red">192.168.1.158</font><br><font color="red">FE80::1</font> |

