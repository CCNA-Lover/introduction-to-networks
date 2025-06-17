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
                    <td>Eth6</td>
                    <td>N/A</td>
                    <td>F0/0</td>
                </tr>
                <tr>
                    <td>Coax7</td>
                    <td>N/A</td>
                    <td>Port0</td>
                </tr>
                <tr>
                      <td rowspan="2">Cable Modem</td>
                      <td>Port0</td>
                      <td>N/A</td>
                      <td>Coax7</td>
                  </tr>
                  <tr>
                      <td>Port1</td>
                      <td>N/A</td>
                      <td>Internet</td>
                  </tr>
                <tr>
                      <td rowspan="4">Router0</td>
                      <td>Comsole</td>
                      <td>N/A</td>
                      <td>RS232</td>
                  </tr>
                  <tr>
                      <td>F0/0</td>
                      <td>192.168.2.1/24</td>
                      <td>Eth6</td>
                  </tr>
                  <tr>
                      <td>F0/1</td>
                      <td>10.0.0.1/24</td>
                      <td>F0</td>
                  </tr>
                  <tr>
                      <td>Ser0/0/0</td>
                      <td>172.31.0.1/24</td>
                      <td>Ser0/0</td>
                  </tr>
                  <tr>
                      <td rowspan="2">Router1</td>
                      <td>Ser0/0</td>
                      <td>172.31.0.2/24</td>
                      <td>Ser0/0/0</td>
                    </tr>
                  <tr>
                      <td>F1/0</td>
                      <td>172.16.0.1/24</td>
                      <td>F0/1</td>
                  </tr>
                <tr>
                      <td rowspan="2">WirelessRouter</td>
                      <td>Internet</td>
                      <td>192.168.2.2/24</td>
                      <td>Port 1</td>
                  </tr>
                  <tr>
                      <td>Eth1</td>
                      <td>192.168.1.1 </td>
                      <td>F0</td>
                  </tr>
                  <tr>
                    <td>Family PC</td>
                    <td>F0</td>
                    <td>192.168.1.102</td>
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
                    <td>10.0.0254</td>
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
