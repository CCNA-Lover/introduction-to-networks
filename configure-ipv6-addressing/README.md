# Background
In this activity, you will practice configuring IPv6 addresses on a router, servers, and clients. You will also practice verifying your IPv6 addressing implementation.
# Objectives
- Configure IPv6 Addressing on the Router
- Configure IPv6 Addressing on Servers
- Configure IPv6 Addressing on Clients
- Test and Verify Network Connectivity
# Addressing Table
<body>
    <div class="container">
        <table>
            <thead>
                <tr>
                    <th>Device</th>
                    <th>Interface</th>
                    <th>IPv6 Address/Prefix</th>
                    <th>Default Gateway</th>
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
                    <td class="device-cell">Billing</td>
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
