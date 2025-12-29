# OPC-UA-SIEMENS-NODE-RED
This project utilizes OPC UA communication configured in TIA Portal in combination with Node-RED.
The objective is to enable efficient data exchange between a Siemens S7-1214C PLC and an S7-1511-1 PN PLC,
with particular emphasis on minimizing data payload size and optimizing data packaging for improved communication efficiency.

# Scenario
Under normal conditions, Node-RED executes OPC UA read/write cycles every 15 s.
Upon an alarm event, the communication cycle is reduced to 1 s to ensure fast data synchronization.
Both the S7-1214C and S7-1511-1 PN operate as OPC UA servers.

# Mesurments 
Network traffic measurements were collected using Wireshark, in both online and offline operating modes, over a duration of 1 minute.

Online mode:                       Offline mode:
Average bytes/s 3685               Average bytes/s 1080
Average bits/s  29k                Average bits/s  8647      






