# Background
In this activity, you will practice configuring IPv6 addresses on a router, servers, and clients. You will also practice verifying your IPv6 addressing implementation.
# Objectives
- Configure IPv6 Addressing on the Router
- Configure IPv6 Addressing on Servers
- Configure IPv6 Addressing on Clients
- Test and Verify Network Connectivity
# Addressing Table
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IPv6 Network Configuration</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', Helvetica, Arial, sans-serif;
            margin: 20px;
            background-color: #f6f8fa;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            border-radius: 6px;
            border: 1px solid #d0d7de;
            overflow: hidden;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            font-size: 14px;
        }
        
        th {
            background-color: #f6f8fa;
            border: 1px solid #d0d7de;
            padding: 8px 12px;
            text-align: left;
            font-weight: 600;
            color: #24292f;
        }
        
        td {
            border: 1px solid #d0d7de;
            padding: 8px 12px;
            color: #24292f;
        }
        
        tr:nth-child(even) {
            background-color: #f6f8fa;
        }
        
        tr:hover {
            background-color: #f1f8ff;
        }
        
        .device-cell {
            font-weight: 600;
            vertical-align: top;
        }
        
        .code {
            font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
            font-size: 12px;
            background-color: rgba(175, 184, 193, 0.2);
            padding: 2px 4px;
            border-radius: 3px;
        }
    </style>
</head>
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
                    <td rowspan="3" class="device-cell">R1</td>
                    <td><span class="code">G0/0</span></td>
                    <td>
                        <span class="code">2001:db8:1:1::1/64</span><br>
                        <span class="code">fe80::1</span>
                    </td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td><span class="code">G0/1</span></td>
                    <td>
                        <span class="code">2001:db8:1:2::1/64</span><br>
                        <span class="code">fe80::1</span>
                    </td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td><span class="code">S0/0/0</span></td>
                    <td>
                        <span class="code">2001:db8:1:a001::2/64</span><br>
                        <span class="code">fe80::1</span>
                    </td>
                    <td>N/A</td>
                </tr>
                <tr>
                    <td class="device-cell">Sales</td>
                    <td>NIC</td>
                    <td><span class="code">2001:db8:1:1::2/64</span></td>
                    <td><span class="code">fe80::1</span></td>
                </tr>
                <tr>
                    <td class="device-cell">Billing</td>
                    <td>NIC</td>
                    <td><span class="code">2001:db8:1:1::3/64</span></td>
                    <td><span class="code">fe80::1</span></td>
                </tr>
                <tr>
                    <td class="device-cell">Accounting</td>
                    <td>NIC</td>
                    <td><span class="code">2001:db8:1:1::4/64</span></td>
                    <td><span class="code">fe80::1</span></td>
                </tr>
                <tr>
                    <td class="device-cell">Design</td>
                    <td>NIC</td>
                    <td><span class="code">2001:db8:1:2::2/64</span></td>
                    <td><span class="code">fe80::1</span></td>
                </tr>
                <tr>
                    <td class="device-cell">Engineering</td>
                    <td>NIC</td>
                    <td><span class="code">2001:db8:1:2::3/64</span></td>
                    <td><span class="code">fe80::1</span></td>
                </tr>
                <tr>
                    <td class="device-cell">CAD</td>
                    <td>NIC</td>
                    <td><span class="code">2001:db8:1:2::4/64</span></td>
                    <td><span class="code">fe80::1</span></td>
                </tr>
                <tr>
                    <td class="device-cell">ISP</td>
                    <td><span class="code">S0/0/0</span></td>
                    <td><span class="code">2001:db8:1:a001::1</span></td>
                    <td><span class="code">fe80::1</span></td>
                </tr>
            </tbody>
        </table>
    </div>
</body>
</html>
