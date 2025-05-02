# Step 1: Configure the initial settings on R1.
a. Configure **R1** as the hostname.<br>
b. Configure Message of the day text: **Unauthorized access is strictly prohibited**.<br>
c. Encrypt all plain text passwords.<br>
Use the following passwords:<br>
1) Privileged EXEC, unencrypted: **cisco**
2) Privileged EXEC, encrypted: **itsasecret**
3) Console: **letmein**

# Step 2: Verify the initial settngs on R1.
a. Verify the initial settings by viewing the configuration for R1.<br>
What command do you use?<br><br>
b. Exit the current console session until you see the following message:<br>
`R1 con0 is now available`<br><br>
`Press RETURN to get started.`<br><br>
c. Press **ENTER**; you should see the following message:<br>
`Unauthorized access is strictly prohibited.`<br><br>
`User Access Verification`<br><br>
`Password:`<br><br>
Why should every router have a message-of-the-day (MOTD) banner?<br>
If you are not prompted for a password before reaching the user EXEC prompt, what console line command did you forget to configure?<br><br>
d. Enter the passwords necessary to return to privileged EXEC mode.<br>
Why would the **enable secret** password allow access to the privileged EXEC mode and **the enable password** no longer be valid?<br>
If you configure any more passwords on the router, are they displayed in the configuration file as plain text or in encrypted form? Explain.
