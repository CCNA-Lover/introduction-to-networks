## Step 1: Verify connectivity.
Ping the following Regional Internet Registry (RIR) websites to verify connectivity:<br>
```C:\Users\User1> ping www.lacnic.net```<br>
```C:\Users\User1> ping www.afrinic.net```<br>
```C:\Users\User1> ping www.apnic.net```<br><br>
**Note**: Because www.ripe.net and www.arin.net do not reply to ICMP requests, they cannot be used for this lab.<br>
If the websites are resolved to IPv6 addresses, the option -4 can be used to resolve to IPv4 addresses if desired. The command becomes **ping -4 www.apnic.net**. 
## Step 2: Collect network data.
You will collect a sufficient amount of data to compute statistics on the **ping** output by sending out 25 echo requests to each address listed in Step 1. This step may require administrative privileges, depending upon your operating system. Record the results for each website to text files.<br><br>
a. At the command prompt, type **ping** to list the available options.
```C:\Users\User1> ping```<br><br>
b. Using the **ping** command with the count option, you can send 25 echo requests to the destination as illustrated below. Furthermore, it will create a text file with filename of **lacnic.txt** in the current directory. This text file will contain the results of the echo requests.
```C:\Users\User1> ping –n 25 www.lacnic.net > lacnic.txt ```<br><br>
**Note**: The terminal remains blank until the command has finished, because the output has been redirected to a text file, **lacnic.txt**, in this example. The **>** symbol is used to redirect the screen output to the file and overwrite the file if it already exists. If appending more results to the file is desired, replace **>** with **>>** in the command.<br><br>
c. Repeat the **ping** command for the other websites.<br>
```C:\Users\User1> ping –n 25 www.afrinic.net > afrinic.txt```<br>
```C:\Users\User1> ping –n 25 www.apnic.net > apnic.txt```
## Step 3:
