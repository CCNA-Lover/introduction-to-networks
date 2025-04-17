## Step 1: Use the tracert command and record the output to text files.
Copy the following commands to create the traceroute files:<br>
`C:\Users\User1> tracert www.lacnic.net > traceroute_lacnic.txt`<br>
`C:\Users\User1> tracert www.afrinic.net > traceroute_afrinic.txt`<br>
`C:\Users\User1> tracert www.apnic.net > traceroute_apnic.txt`<br>
**Note**:  If the websites are resolved to IPv6 addresses, the option **-4** can be used to resolve to IPv4 addresses if desired. The command becomes `tracert -4 www.lacnic.net > traceroute_lacnic.txt`. 
## Step 2: Use the more command to examine the traced path.
a. Use the **more** command to access the content of these files:<br>
`C:\Users\User1> more traceroute_lacnic.txt`
In this example, it took less than 1 ms to receive a reply from the default gateway (192.168.0.1). In hop count 6, the round trip to 4.28.58.177 took an average of 37 ms. For the round trip to the final destination at www.lacnic .net took an average of 225 ms.<br><br>
Between lines 8 and 9, there is more network delay as indicated by the round trip time increase from an average of 78 ms to 298 ms
b. Perform the same analysis with the rest of the tracert results.<br><br>
What can you conclude regarding the relationship between the roundtrip time and geographical location?
