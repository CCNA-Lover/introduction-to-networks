## Step 1: Verify the network documentation and isolate any problems.
a. Before you can effectively test a network, you must have complete documentation. Notice in the **Addressing Table** that some information is missing. Complete the **Addressing Table** by filling in the missing default gateway information for the switches and the PCs. <br><br>
b. Test connectivity to devices on the same network. By isolating and correcting any local access issues, you can better test remote connectivity with the confidence that local connectivity is operational.<br>
A verification plan can be as simple as a list of connectivity tests. Use the following tests to verify local connectivity and isolate any access issues. The first issue is already documented, but you must implement and verify the solution during Part 2.
**Testing and Verification Documentation**
|Test|Successful?|Issues|Solution|Verified|
|:---:|:---:|:---:|:---:|:---:|
|PC1 to PC2|No|IP address on PC1|Change PC1 IP address||
|PC1 to S1|||||
|PC1 to R1|||||
||||||
||||||

**Note**: The table is an example; you must create your own document. You can use paper and pencil to draw a table, or you can use a text editor or spreadsheet. Consult your instructor if you need further guidance.<br><br>
c. Test connectivity to remote devices (such as from PC1 to PC4) and document any problems. This is frequently referred to as end-to-end connectivity. This means that all devices in a network have the full connectivity allowed by the network policy.<br><br>
**Note**: Remote connectivity testing may not be possible yet, because you must first resolve local connectivity issues. After you have solved those issues, return to this step and test connectivity between networks.
## Determine an appropriate solution for the problem.
a. Using your knowledge of the way networks operate and your device configuration skills, search for the cause of the problem. For example, S1 is not the cause of the connectivity issue between PC1 and PC2. The link lights are green and no configuration on S1 would cause traffic to not pass between PC1 and PC2. So the problem must be with PC1, PC2, or both.<br><br>
b. Verify the device addressing to ensure it matches the network documentation. For example, the IP address for PC1 is incorrect as verified with the **ipconfig** command.<br><br>
c. Suggest a solution that you think will resolve the problem and document it. For example, change the IP address for PC1 to match the documentation.<br><br>
**Note**: Often there is more than one solution. However, it is a troubleshooting best practice to implement and verify one solution at a time. Implementing more than one solution could introduce additional issues in a more complex scenario.

