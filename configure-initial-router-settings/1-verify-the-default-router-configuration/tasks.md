# Step 1: Establish a console connection to R1.
a. CHoose a **Console** cable from the available connections.<br>
b. Click **PCA** and select **RS 232**.<br>
c. Click **R1** and select **Console**.<br>
d. Click **PCA** > **Desktop** tab > **Terminal**.<br>
e. Click **OK** and press **ENTER**. You are now able to configure **R1**.

# Step 2: Enter privileged mode and examine the current configuration.
You can access all the router commands from privileged EXEC mode. However, because many of the privileged commands configure operating parameters, privileged access should be password-protected to prevent unauthorized use.<br><br>
a. Enter privileged EXE mode by entering the **enable** command. You can also type in **en** and hit **ENTER** - the autocompletion feature of the CLI will automatically write the **enable** command out.<br>
```Router> enable```<br>
```Router#```<br>
Notice that the prompt changed in the configuration to reflect privileged EXEC mode.<br><br>
b. Enter the **show running-config** command. Alternatively you can just write **sh run** and hit **ENTER** - the autocompletion feature will understand you meant the *show running-config* command.<br>
`Router# show running-config`<br>
What is the router's name?<br>
How many Fast Ethernet interfaces does the Router have?<br>
How many Gigabit Ethernet interfaces does the Router have?<br>
How many Serial interfaces does the router have?<br>
What is the range of values shown for the vty lines?<br><br>
c. Display the currect contents of the NVRAM.<br>
`Router# show startup-config`<br>
As for the running configuration file (stored in the RAM), you can also display the content of the startup configuration file (stored in the Non Volatile RAM - it is the config file that is booted up by default when the router gets on) just by using the shortened form of the command: *sh start*.<br>
Why does the router respond with the **startup-config is not present message**?
