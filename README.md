# Multi-Site-Corporate-Network

<img width="1365" height="723" alt="image" src="https://github.com/user-attachments/assets/0030108e-4e89-4bec-a9cb-92d0f89e9391"/>

<h2>Description</h2>
I designed a three site network connecting a Headquarter (HQ-Router) to two remote offices branch 1 and branch 2 routers in Cisco Packet Tracer. Configured with inter-site WAN links alongside local area networks at each location using switches and end user PC(PC0–PC5). A DHCP server was deployed Headquarters site to automate IP address assignment.

<h2>Languages and Utilities Used</h2>

- <b>Packet Tracer</b> 

<h2>Environments Used </h2>

- <b>Windows 11 </b> (26H2)

<h2>Project Walkthrough </h2>

<p align="center">
Topology design and cabling: <br/>
<img width="1365" height="701" alt="image" src="https://github.com/user-attachments/assets/8e66ab12-0576-4829-9c5c-bebb913df0ac" 
 style="width: 600px; max-width: 100%; height: auto;"/>
<h3>WAN vs LAN subnet design</h3>
The WAN links use a /30 subnet mask (255.255.255.252), whereas LANs typically use a /24 (255.255.255.0), because point-to-point WAN links only ever need two usable IP addresses.
<br />
<br />
 <h3>DHCP with Cross-Site Relay:  </h3><br/>
 
 DHCP server and relay setup

In this step, I’m setting up DHCP so that devices at all sites can recieve IP addresses and DHCP relay is used tomforward  DHCP messages between client devices and DHCP servers located on different subnets or networks.

<p align="center">
Network topology with DHCP server and PCs at each site<br/>
<img width="1365" height="579" alt="image" src="https://github.com/user-attachments/assets/afec9c9e-2812-4e32-a15d-fc221bfafabd" 



<br />
<br />
Enter the number of passes: <br/>

<br />
<br />
Confirm your selection:  <br/>

<br />
<br />
Wait for process to complete (may take some time):  <br/>

<br />
<br />
Sanitization complete:  <br/>

<br />
<br />
Observe the wiped disk:  <br/>

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
