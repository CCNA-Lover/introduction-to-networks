## Step 1: Use ipv6config and ping to verify connectivity.
a. Click **PC2** and open the **Command Prompt**.<br><br>
b. Enter the **ipv6config /all** command to collect the IPv6 information. Complete the **Addressing Table** with the IPv6 address, subnet mask, and default gateway.<br><br>
c. Click **PC4** and open the **Command Prompt**.<br><br>
d. Enter the **ipv6config /all** command to collect the IPv6 information. Complete the **Addressing Table** with the IPv6 address, subnet mask, and default gateway.<br><br>
e. Test connectivity between **PC2** and **PC4**. The ping should fail.
## Step 2: Locate the source of connectivity failure.
a. From **PC2**, enter the necessary command to trace the route to **PC4**.<br><br>
What is the last successful IPv4 address that was reached?<br><br>
b. The trace will eventually end after 30 attempts. Enter **Ctrl+C** to stop the trace before 30 attempts.<br><br>
c. From **PC4**, enter the necessary command to trace the route to **PC2**.<br><br>
What is the last successful IPv6 address that was reached?<br><br>
d. Enter **Ctrl+C** to stop the trace.<br><br>
e. Click **R3**. Press **ENTER** and log in to the router.<br><br>
f. Enter the **show ipv6 interface brief** command to list the interfaces and their status. There are two IPv6 addresses on the router. One should have been recorded in Step 1d.<br><br>
Is there a discrepancy?<br><br>
g. Run more tests if it helps visualize the problem. Simulaiton mode is available.
## Step 3:Propose a solution to the problem.
Compare your answers in Step 2 to the documentation you have available for the network.<br><br>
What is the error?<br><br>
What solution would you propose to correct the problem?
## Step 4: Implement the plan.
Implement the solution you proposed in Step 3b.
## Step 5: Verify that connectivity is restored.
a. From **PC2** test connectivity to **PC4**.<br><br>
b. From **PC4** test connectivity to **PC2**.<br><br>
Is the problem resolved?
## Step 6: Document the solution.
