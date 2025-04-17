## Step 1: Enter privileged EXEC mode.
a. At the prompt, type the question mark (**?**).<br>
`S1> ?`<br>
What information is displayed for the **enable** command?<br><br>
b. Type **en** and press the **Tab** key.<br>
`S1> en<Tab>`<br>
What displays after pressing the **Tab** key?<br><br>
Tis is called command (or tab completion). WHen part of a command is typed, the **Tab** key can be used to continue the partial command. If the characters typed are enough to make the command unique, as in the case of the **enable** command, the remaining portion of the command is displayed.<br>
What would happen if you typed **te<Tab>** at the prompt?<br><br>
c. Enter the **enable** command and press ENTER.<br>
How does the prompt change?<br><br>
d. When prompted, type the question mark (**?**).<br><br>
`S1# ?`<br>
One command starts with the letter 'C' in user EXEC mode.<br>
How many commands are displayed now that privileged EXEC mode is active? (**Hint**: you could type *c?* to list just the commands beginning with 'C'.)
## Step 2: Enter Global Configuration mode
a. When in privileged EXEC mode, one of the commands starting with the letter ‘C’ is **configure**. Type either the full command or enough of the command to make it unique. Press the <**Tab**> key to issue the command and press ENTER.<br>
`S1# configure`<br>
What is the message that is displayed?<br><br>
b. Press Enter to accept the default parameter that is enclosed in brackets **[terminal]**.<br>
How does the prompt change?<br><br>
c. This is called global configuration mode. This mode will be explored further in upcoming activities and labs. For now, return to privileged EXEC by typing **end**, **exit** or **Ctrl-Z**.<br>
`S1(config)# exit`
`S1#`
