## Step 1: Verify connectivity.
Ping the following Regional Internet Registry (RIR) websites to verify connectivity:<br>
```C:\Users\User1> ping www.lacnic.net```<br>
```C:\Users\User1> ping www.afrinic.net```<br>
```C:\Users\User1> ping www.apnic.net```<br><br>
**Note**: Because www.ripe.net and www.arin.net do not reply to ICMP requests, they cannot be used for this lab.<br>
If the websites are resolved to IPv6 addresses, the option **-4** can be used to resolve to IPv4 addresses if desired. The command becomes ```ping -4 www.apnic.net```. 
## Step 2: Collect network data.
You will collect a sufficient amount of data to compute statistics on the **ping** output by sending out 25 echo requests to each address listed in Step 1. This step may require administrative privileges, depending upon your operating system. Record the results for each website to text files.<br><br>
a. At the command prompt, type **ping** to list the available options.
```C:\Users\User1> ping```<br><br>
b. Using the **ping** command with the count option, you can send 25 echo requests to the destination as illustrated below. Furthermore, it will create a text file with filename of **lacnic.txt** in the current directory. This text file will contain the results of the echo requests.<br>
```C:\Users\User1> ping –n 25 www.lacnic.net > lacnic.txt ```<br><br>
**Note**: The terminal remains blank until the command has finished, because the output has been redirected to a text file, **lacnic.txt**, in this example. The **>** symbol is used to redirect the screen output to the file and overwrite the file if it already exists. If appending more results to the file is desired, replace **>** with **>>** in the command.<br><br>
c. Repeat the **ping** command for the other websites.<br>
```C:\Users\User1> ping –n 25 www.afrinic.net > afrinic.txt```<br>
```C:\Users\User1> ping –n 25 www.apnic.net > apnic.txt```
## Step 3: Verify data collection.
To verify that the files have been created, use the **dir** command to list the files in the directory. Also the wildcard * can be used to filter only the text files.<br>
```C:\Users\User1> dir *.txt```<br><br>
To see the results in the file created, use the **more** command at the command prompt.<br>
```C:\Users\User1> more lacnic.txt``` <br><br>
**Note**:  Press the Spacebar to display the rest of the file or press **q** to exit.<br>
Record your results in the following table.
||Minimum|Maximum|Average|
|:---:|:---:|:---:|:---:|
|`www.afrinic.net`||||
|`www.apnic.net`||||
|`www.lacninc.net`||||

Compare the delay results. How is delay affected by geographical location?
