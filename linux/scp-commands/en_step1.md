## Problem - SCP command
In this scenario, you are requested to access the specified file directory on the machines allocated to you and prepare a scenario in which you apply the file transfer operations with the SCP command in accordance with the instructions below.
### Information
SCP COMMAND:

SCP stands for "Secure Copy Protocol" and is a network protocol used for file transfer. SCP is used to securely copy or move files between computers. This protocol provides encryption and secure transfer of data.

SCP is a command line tool mostly used on UNIX and Linux operating systems.

In this scenario, we will transfer files between different nodes.

### Instructions
1. Go to `/home` directory on node1 and node2 servers.
2. Create `exp.txt` files on node1 server and `expm.txt` files on node2 server.
3. Send expm.txt file from node2 server to node1 server via `SCP` command.
4. With the SCP command, after answering the security question YES while transferring files between servers, you can check that the file transfer is successful and then come to the node1 server and check that the `expm.txt` file exists.
5. After completing the procedures, click the "Check" button and complete the scenario.

### Successful Output
  Condition:
`` echo
[root@node1 ~]$ cat backup.sql
```