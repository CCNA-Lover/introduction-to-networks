
# Addressing Table
<body>
    <div>
        <table>
            <thead>
                <tr>
                    <th>Device</th>
                    <th>Interface</th>
                    <th>IP Address</th>
                    <th>Connects To</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td rowspan="3">R1</td>
                    <td><span>G0/0</span></td>
                    <td>
                        <span>2001:db8:1:1::1/64</span><br>
                        <span>fe80::1</span>
                    </td>
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
- Part 1: Connect to the Cloud
- Part 2: Connect Router0
- Part 3: Connect Remaining Devices
- Part 4: Verify Connections
- Part 5: Examine the Physical Topology 

# Background
When working in Packet Tracer (a lab environment or a corporate setting), you should know how to select the appropriate cable and how to properly connect devices. This activity will examine device configurations in Packet Tracer, selecting the proper cable based on the configuration, and connecting the devices. This activity will also explore the physical view of the network in Packet Tracer.
