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
                    <td>G0/1</td>
                    <td>192.168.11.1</td>
                    <td>255.255.255.0</td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td>S0/0/0 (DCE)</td>
                    <td>209.165.200.225</td>
                    <td>255.255.255.252</td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td rowspan="3">R2</td>
                    <td>G0/0</td>
                    <td>10.1.1.1</td>
                    <td>255.255.255.0</td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td>G0/1</td>
                    <td>10.1.2.1</td>
                    <td>255.255.255.0</td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td>S0/0/0</td>
                    <td>209.165.200.226</td>
                    <td>255.255.255.252</td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td>PC1</td>
                    <td>NIC</td>
                    <td>192.168.10.10</td>
                    <td>255.255.255.0</td>
                    <td>192.168.10.1</td>
                </tr>
                <tr>
                    <td>PC2</td>
                    <td>NIC</td>
                    <td>192.168.11.10</td>
                    <td>255.255.255.0</td>
                    <td>192.168.11.1</td>
                </tr>
                <tr>
                    <td>PC3</td>
                    <td>NIC</td>
                    <td>10.1.1.10</td>
                    <td>255.255.255.0</td>
                    <td>10.1.1.1</td>
                </tr>
                <tr>
                    <td>PC4</td>
                    <td>NIC</td>
                    <td>10.1.2.10</td>
                    <td>255.255.255.0</td>
                    <td>10.1.2.1</td>
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
