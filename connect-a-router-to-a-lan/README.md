# Addressing Table
<body>
    <div>
        <table>
            <thead>
                <tr>
                    <th>Device</th>
                    <th>Interface</th>
                    <th>IP Address</th>
                    <th>Subnet Mask</th>
                    <th>Default Gateway</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td rowspan="3">R1</td>
                    <td>G0/0</td>
                    <td>192.168.10.1</td>
                    <td>255.255.255.0</td>
                    <td>N/A</td>
                </tr>
                <tr>
                      <td rowspan="3">R2</td>
                      <td>G0/0</td>
                      <td>192.168.11.1</td>
                      <td>255.255.255.0</td>
                      <td>N/A</td>
                  </tr>
                <tr>
                    <td><span>G0/1</span></td>
                    <td>
                        <span>2001:db8:1:2::1/64</span><br>
                        <span>fe80::1</span>
                    </td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td><span>S0/0/0</span></td>
                    <td>
                        <span>2001:db8:1:a001::2/64</span><br>
                        <span>fe80::1</span>
                    </td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td>Sales</td>
                    <td>NIC</td>
                    <td><span>2001:db8:1:1::2/64</span></td>
                    <td><span>fe80::1</span></td>
                </tr>
                <tr>
                    <td>Billing</td>
                    <td>NIC</td>
                    <td><span>2001:db8:1:1::3/64</span></td>
                    <td><span>fe80::1</span></td>
                </tr>
                <tr>
                    <td>Accounting</td>
                    <td>NIC</td>
                    <td><span>2001:db8:1:1::4/64</span></td>
                    <td><span>fe80::1</span></td>
                </tr>
                <tr>
                    <td>Design</td>
                    <td>NIC</td>
                    <td><span>2001:db8:1:2::2/64</span></td>
                    <td><span>fe80::1</span></td>
                </tr>
                <tr>
                    <td>Engineering</td>
                    <td>NIC</td>
                    <td><span>2001:db8:1:2::3/64</span></td>
                    <td><span>fe80::1</span></td>
                </tr>
                <tr>
                    <td>CAD</td>
                    <td>NIC</td>
                    <td><span>2001:db8:1:2::4/64</span></td>
                    <td><span>fe80::1</span></td>
                </tr>
                <tr>
                    <td>ISP</td>
                    <td><span>S0/0/0</span></td>
                    <td><span>2001:db8:1:a001::1</span></td>
                    <td><span>fe80::1</span></td>
                </tr>
            </tbody>
        </table>
    </div>
</body>


# Objectives
- Part 1: Display Router Information
- Part 2: Configure Router Interfaces
- Part 3: Verify the Configuration

# Background
In this activity, you will use various show commands to display the current state of the router. You will then use the Addressing Table to configure router Ethernet interfaces. Finally, you will use commands to verify and test your configurations. Note: The routers in this activity are partially configured. Some of the configurations are not covered in this course but they are provided to assist you in using verification commands. 
