# Step 1: Establish a console connection to R1.
a. CHoose a **Console** cable from the available connections.<br>
b. Click **PCA** and select **RS 232**.<br>
c. Click **R1** and select **Console**.<br>
d. Click **PCA** > **Desktop** tab > **Terminal**.<br>
e. Click **OK** and press **ENTER**. You are now able to configure **R1**.

# Step 2: Enter privileged mode and examine the current configuration.
You can access all the router commands from privileged EXEC mode. However, because many of the privileged commands configure operating parameters, privileged access should be password-protected to prevent unauthorized use.<br>
a. Enter privileged EXE mode by entering the **enable** command. You can also type in **en** and hit **ENTER** - the autocompletion feature of the CLI will automatically write the **enable** command out.<br>
```Router> enable```<br>
```Router#```<br>
Notice that the prompt changed in the configuration to reflect privileged EXEC mode.<br>
b. Enter the **show running-config** command. Alternatively you can just write **sh run** and hit **ENTER** - the autocompletion feature will understand you meant the *show running-config* command.<br>
`Router# show running-config`<br>
What is the router's name?
