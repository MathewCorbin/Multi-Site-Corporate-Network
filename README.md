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
 <h3>DHCP with Cross-Site Relay:  </h3>
 DHCP server and relay setup
 
In this step, I’m setting up DHCP so that devices at all sites can recieve IP addresses and DHCP relay is used to forward  DHCP messages between client devices and DHCP servers located on different subnets or networks.

<p align="center">
Network topology with DHCP server and PCs at each site<br/>
<img width="1365" height="579" alt="image" src="https://github.com/user-attachments/assets/afec9c9e-2812-4e32-a15d-fc221bfafabd"  style="width: 600px; max-width: 100%; height: auto;"/>

<br />

 <h3>Delivering DNS and Internal Web Services</h3>
 <p align="center">
  In this step, I’m setting up DNS so that I can access the company webpage from branch2
<img width="1365" height="703" alt="image" src="https://github.com/user-attachments/assets/0340e5a4-bf55-4452-a107-240d1f6eb9b8"
  style="width: 600px; max-width: 100%; height: auto;"/>
  
<p align="center">
Network topology with DNS Server and PCs<br/>
  <img width="1363" height="719" alt="image" src="https://github.com/user-attachments/assets/4ea1f78e-ad33-4b8f-9f73-5ac1a0f3558d"
     style="width: 600px; max-width: 100%; height: auto;"/>


<br />
<br />
<h1>Reflections and Takeaways</h1>
 <h3>Time and challenges</h3>
 In total this project took me about 1.5 hrs to do because I encountered an error where branch2 PCs weren't able to send DHCP request to the DHCP server due to IP misconfiguration on the router. After troubleshooting I discovered that Branch2Router had no route to HQ and HQ-Router & Branch1-Router had no return routes to Branch 2's LAN. After correcting this mistake everything worked perfectly

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
