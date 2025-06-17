
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
                    <td rowspan="2">Cloud</td>
                    <td>
                        <span>Eth6</span><br>
                        <span>Coax7</span>
                    </td>
                    <td>
                        <span>N/A</span><br>
                        <span>N/A</span>
                    </td>
                    <td>
                        <span>F0/0</span><br>
                        <span>Port0</span>
                    </td>
                </tr>
                <tr>
                    <td rowspan="2">Cable Modem</td>
                    <td>
                        <span>Port0</span><br>
                        <span>Port1</span>
                    </td>
                    <td>
                        <span>N/A</span><br>
                        <span>N/A</span>
                    </td>
                    <td>
                        <span>Coax7</span><br>
                        <span>Internet</span>
                    </td>
                </tr>
                <tr>
                    <td rowspan="4">Router0</td>
                    <td>
                        <span>Console</span><br>
                        <span>F0/0</span>
                        <span>F0/1</span>
                        <span>Ser0/0/0</span>
                    </td>
                    <td>
                        <span>N/A</span><br>
                        <span>192.168.2.1/24</span>
                        <span>10.0.0.1/24</span>
                        <span>173.31.0.1/24</span>
                    </td>
                    <td>
                        <span>RS232</span><br>
                        <span>Eth6</span>
                        <span>F0</span>
                        <span>Ser0/0</span>
                    </td>
                </tr>
                <tr>
                    <td rowspan="2">Router1</td>
                    <td>
                        <span>Ser0/0</span><br>
                        <span>F1/0</span>
                    </td>
                    <td>
                        <span>172.31.0.2/24</span><br>
                        <span>172.16.0.1/24</span>
                    </td>
                    <td>
                        <span>Ser0/0/0</span><br>
                        <span>F0/1</span>
                    </td>
                </tr>
                <tr>
                    <td rowspan="2">WirelessRouter</td>
                    <td>
                        <span>Internet</span><br>
                        <span>Eth1</span>
                    </td>
                    <td>
                        <span>192.168.2.2/24</span><br>
                        <span>192.168.1.1</span>
                    </td>
                    <td>
                        <span>Port1</span><br>
                        <span>F0</span>
                    </td>
                </tr>
                <tr>
                    <td>Family PC</td>
                    <td>F0</td>
                    <td>192.168.1.1</td>
                    <td>Eth1</td>
                </tr>
                <tr>
                    <td>Switch</td>
                    <td>F0/1</td>
                    <td>172.16.0.2</td>
                    <td>F1/0</td>
                </tr>
                <tr>
                    <td>Netacad.pka</td>
                    <td>F0</td>
                    <td>10.0.0.254</td>
                    <td>F0/1</td>
                </tr>
                <tr>
                    <td>Configuration Terminal</td>
                    <td>RS232</td>
                    <td>N/A</td>
                    <td>Console</td>
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
