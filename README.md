# Network-Security-Groups-and-Inspecting-Traffic-between-Azure-WM-s
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/PC)
- Remote Desktop
- Powershell and Command 
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create Windows 10 WM and Linux Ubuntu Server within Azure
- Use Remote Desktop and download Wireshark on WM1
- Ping WM 2's IP address to verify connectivity
- Block WM 1's firewall and observe the closed traffic
- Observe all traffic on ICMP, SSH, DNS, and RDP protocols

<h2>Actions and Observations</h2>
<p>
<img src="https://imgur.com/2I33krA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Installed Wireshark on WM1!
</p>
<br />
&emsp;
&emsp;
&emsp;
&emsp;


<img src="https://imgur.com/c25gO4E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
-Inspected traffic between both of the virtual machines. Wireshark gives the option to filter which networking protocol to use, I observed the traffic with ICMP.
 </p>
<br />

&emsp; 
&emsp;
&emsp;              
<img src="https://imgur.com/TweMPvW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
-Created a new inbound rule within Azure to  ban all ICMP4 traffic.
 </p>
<br />
&emsp; 
&emsp;
<img src="https://imgur.com/QBbEbNt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 - Inbound rule in motion. No replies from WM2!
