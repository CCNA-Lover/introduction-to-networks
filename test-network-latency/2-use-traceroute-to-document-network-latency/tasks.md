## Step 1: Use the tracert command and record the output to text files.
Copy the following commands to create the traceroute files:<br>
`C:\Users\User1> tracert www.lacnic.net > traceroute_lacnic.txt`<br>
`C:\Users\User1> tracert www.afrinic.net > traceroute_afrinic.txt`<br>
`C:\Users\User1> tracert www.apnic.net > traceroute_apnic.txt`<br><br>
**Note**:  If the websites are resolved to IPv6 addresses, the option **-4** can be used to resolve to IPv4 addresses if desired. The command becomes `tracert -4 www.lacnic.net > traceroute_lacnic.txt`. 
## Step 2: Use the more command to examine the traced path.
a. Use the **more** command to access the content of these files:<br>
`C:\Users\User1> more traceroute_lacnic.txt`<br><br>
b. Perform the same analysis with the rest of the tracert results.<br><br>
What can you conclude regarding the relationship between the roundtrip time and geographical location?
