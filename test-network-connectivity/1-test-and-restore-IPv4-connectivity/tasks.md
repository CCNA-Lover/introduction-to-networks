## Step 1: Use ipconfig and ping to verify connectivity.
## Step 2: Locate the source of connectivity failure.
a. From **PC1**, enter the necessary command to trace the route to **PC3**.<br><br>
What is the last successful IPv4 address that was reached?<br><br>
b. The trace will eventually end after 30 attempts. Enter **Ctrl+C** to stop the trace before 30 attempts.<br><br>
c. From **PC3**, enter the necessary command to trace the route to **PC1**.<br><br>
What is the last successful IPv4 address that was reached?<br><br>
d. Enter **Ctrl+C** to stop the trace.<br><br>
e. Click **R1**. Press **ENTER** and log in to the router.<br><br>
f. Enter the **show ip interface brief** command to list the interfaces and their status. There are two IPv4 addresses on the router. One should have been recorded in Step 2a.<br><br>
What is the other?<br><br>
g. Enter the **show ip route** command to list the networks to which the router is connected. Note that there are two networks connected to the **Serial0/0/1** interface.<br><br>
What are they?<br><br>
h. Repeat steps 2e through 2g with **R3** and record your answers.<br><br>
i. Click **R2**. Press **ENTER** and log into the router.<br><br>
j. Enter the **show ip interface brief** command and record your addresses. Type your addresses here.<br><br>
k. Run more tests if it helps visualize the problem. Simulation mode is available. 
## Step 3: Propose a solution to solve the problem.
Compare your answers in Step 2 to the documentation you have available for the network.<br><br>
What is the error?<br><br>
What solution would you propose to correct the problem?
## Step 4: Implement the plan.
Implement the solution you proposed in Step 3b.
## Step 5: Verify that connectivity is restored.
a. From PC1 test connectivity to PC3.<br><br>
b. From PC3 test connectivity to PC1.<br><br>
Is the problem resolved?
## Step 6: Document the solution.
