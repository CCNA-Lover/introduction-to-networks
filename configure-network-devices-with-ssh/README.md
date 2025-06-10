# Scenario
The network administrator has asked you to prepare **RTA** and **SW1** for deployment. Before they can be connected to the network, security measures must be enabled. 

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
                    <td>RTA</td>
                    <td>G0/0</td>
                    <td>172.16.1.1</td>
                    <td>255.255.255.0</td>
                    <td>N/A</td>
                </tr>
               <tr>
                    <td>PCA</td>
                    <td>NIC</td>
                    <td>172.16.1.10</td>
                    <td>255.255.255.0</td>
                    <td>172.16.1.1</td>
                </tr>
                <tr>
                    <td>SW1</td>
                    <td>VLAN 1</td>
                    <td>172.16.1.2</td>
                    <td>255.255.255.0</td>
                    <td>172.16.1.1</td>
                </tr>
            </tbody>
        </table>
    </div>
</body>

![image](https://github.com/user-attachments/assets/60d16e36-9b7c-44ef-8c8f-b1135d516754)
