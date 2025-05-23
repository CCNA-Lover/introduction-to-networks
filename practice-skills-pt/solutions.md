# Step 1: Determine the IP Addressing Scheme.

<table>
  <thead>
    <tr>
      <th>Device</th>
      <th>Interface</th>
      <th>IP Address/Mask</th>
      <th>Default Gateway</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">Town Hall</td>
      <td>G0/0</td>
      <td>
        <font color="red">192.168.1.126/27</font><br>
        <font color="red">(SM: 255.255.255.224)</font><br>
        2001:db8:acad:a::1/64<br>
        fe80::1
      </td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>G0/1</td>
      <td>
        <font color="red">192.168.1.158/28</font><br>
        <font color="red">(SM: 255.255.255.240)</font><br>
        2001:db8:acad:b::1/64<br>
        fe80::1
      </td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>Administration Switch</td>
      <td>SVI</td>
      <td>
        <font color="red">192.168.1.157/28</font><br>
        <font color="red">(SM: 255.255.255.240)</font>
      </td>
      <td><font color="red">192.168.1.158</font></td>
    </tr>
    <tr>
      <td>Reception Host</td>
      <td>NIC</td>
      <td>
        <font color="red">192.168.1.97/27</font><br>
        <font color="red">(SM: 255.255.255.224)</font><br>
        2001:db8:acad:a::ff/64
      </td>
      <td>
        <font color="red">192.168.1.126</font><br>
        <font color="red">FE80::1</font>
      </td>
    </tr>
    <tr>
      <td>Operator Host</td>
      <td>NIC</td>
      <td>
        <font color="red">192.168.1.98/27</font><br>
        <font color="red">(SM: 255.255.255.224)</font><br>
        2001:db8:acad:a::15/64
      </td>
      <td>
        <font color="red">192.168.1.126</font><br>
        <font color="red">FE80::1</font>
      </td>
    </tr>
    <tr>
      <td>IT Host</td>
      <td>NIC</td>
      <td>
        <font color="red">192.168.1.145/28</font><br>
        <font color="red">(SM: 255.255.255.240)</font><br>
        2001:db8:acad:b::ff/64
      </td>
      <td>
        <font color="red">192.168.1.158</font><br>
        <font color="red">FE80::1</font>
      </td>
    </tr>
    <tr>
      <td>Server</td>
      <td>NIC</td>
      <td>
        <font color="red">192.168.1.146/28</font><br>
        <font color="red">(SM: 255.255.255.240)</font><br>
        2001:db8:acad:b::15/64
      </td>
      <td>
        <font color="red">192.168.1.158</font><br>
        <font color="red">FE80::1</font>
      </td>
    </tr>
  </tbody>
</table>


