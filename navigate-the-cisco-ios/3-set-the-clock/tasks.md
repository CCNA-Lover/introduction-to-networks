## Step 1: Use the clock command.
a. Use the **clock** command to further explore Help and command syntax. Type **show clock** at the privileged EXEC prompt.<br>
`S1# show clock`<br>
What information is displayed? What is the year that is displayed?<br><br>
b. Use the context-sensitive help ans the **clock** command to set the time on the switch to the current time. Enter the command **clock** and press ENTER.<br>
`S1# clock<ENTER>`<br>
What information is displayed?<br><br>
c. The "% Incomplete command" message is returned by the IOS. This indicates that the **clock** command needs more parameters. Any time more information is needed, help can be provided by typing a space after he command and the question mark (?).<br>
`S1# clock ?`<br>
WWhat information is displayed?<br><br>
d. Set the clock using the **clock set** command. Proceed through the command one step at a time.<br>
`S1# clock set ?`<br>
What information is being requested?<br>
What would have been displayed if only the **clock set** command had been entered, and no request for help was made by using the question mark?<br><br>
e. Based on the information requested by issuing the **clock set ?** command, enter a time of 3:00 p.m. by using the 24-hour format of 15:00:00. Check to see if more parameters are needed.<br>
`S1# clock set 15:00:00 ?`<br><br>
The output returns a request for more information:<br>
`<1-31> Day of the month`<br>
`MONTH Month of the year`<br><br>
f. Attempt to set the date to 01/31/2035 using the format requested. It may be necessary to request additional help using context-sensitive help to complete the process. When finished, issue the **show clock** command to display the clock setting. The resulting command output should display as:<br>
`S1# show clock`<br>
`*15:0:4.869 UTC Tue Jan 31 2035`<br><br>
g. If you were not successful, try te following command to obtain the output above:<br>
`S1# clock set 15:00:00 31 Jan 2035`
## Step 2: Explore additional command messages.
a. The IOS provides various outputs for incorrect or incomplete commands. Continue to use the **clock** command to explore additional messages that may be encountered as you learn to use the IOS.<br><br>
b. Issue the following commands and record the messages:<br>
`S1# cl<tab>`<br>
What information was returned?<br><br>
`S1# clock`<br>
What information was returned?<br><br>
`S1# clock set 25:00:00`<br>
What information was returned?<br><br>
`S1# clock set 15:00:00 32`<br>
What information was returned? 
