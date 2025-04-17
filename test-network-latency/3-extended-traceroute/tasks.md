Although **traceroute** has different implementations depending on the platform, all versions allow the user to adjust its behavior. In Windows, this can be done providing options and switches in the tracert command line.<br><br>
a. Reverse name resolution (resolving an IP address to a domain name) can add a delay to **tracert** results and yield inaccurate results. To ensure **tracert** won’t attempt to reverse resolve hop IP addresses, add the **–d** option to the **tracert** command line:<br>
`C:\Users\User1> tracert –d www.lacnic.net > traceroute_d_lacnic.txt`<br>
`C:\Users\User1> tracert –d www.afrinic.net > traceroute_d_afrinic.txt`<br>
`C:\Users\User1> tracert –d www.apnic.net > traceroute_d_apnic.txt`<br><br>
b.Use the **more** command to access the content of these files:<br>
`C:\Users\User1> more traceroute_d_lacnic.txt`<br>
What is different about the **tracert** output when the **-d** option was added?<br><br>
**Note**: Windows **tracert** will present a list of available options and their descriptions when issued without any options.<br><br>
**Note**: Cisco IOS implementation of **traceroute** also allows for fine tuning but it does not rely on command line options. Cisco IOS extended traceroute presents a number of simple questions to allow the administrator to provide values for the desired parameters.

## Reflection Questions
1. The **tracert** and **ping** results can provide important network latency information. What do you need to do if you want an accurate baseline picture regarding network latency for your network? Type your answers here.<br><br>
2. How can you use the baseline information? 
