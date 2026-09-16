# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Nmae : KATHIRAVAN B
# Reg No: 212223060117
# Date: 5/8/26
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
<img width="1920" height="1080" alt="Screenshot (141)" src="https://github.com/user-attachments/assets/e985a8c9-677f-4e48-9ecf-de6beba9f2f4" />

________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>

<img width="1920" height="1080" alt="Screenshot (136)" src="https://github.com/user-attachments/assets/d3bbed60-c00a-4224-b8f0-b8f34dee9f16" />
<img width="1920" height="1080" alt="Screenshot (135)" src="https://github.com/user-attachments/assets/30344006-55fd-4d0f-8b7c-d045210f1972" />
<img width="1920" height="1080" alt="Screenshot (134)" src="https://github.com/user-attachments/assets/2861857e-552b-43d4-88f0-9a07025408c3" />

•	PDU details for remote communication<br>
<img width="1920" height="1080" alt="Screenshot (138)" src="https://github.com/user-attachments/assets/6359975f-be4e-47b3-b221-2b0d520b0b33" />
<img width="1920" height="1080" alt="Screenshot (139)" src="https://github.com/user-attachments/assets/4df8f5bc-ff58-455e-9f64-6f57fe0905d6" />

•	Tables showing MAC/IP changes through each device<br>
<img width="1920" height="1080" alt="Screenshot (140)" src="https://github.com/user-attachments/assets/9ecff0bf-5c6a-4742-8ff0-ff148fd616bc" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

