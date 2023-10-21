# NSG's and Inspecting Traffic between Azure virtual machines
<h2>Environments and Technologies Used</h2>

- Virtual Machines hosted on Azure 
- Windows 10 (21H2)
- _Ubuntu Server 20.04_
- _Microsoft Remote Desktop_
- _Powershell and Command_ 
- Network Protocols (**SSH**, **RDH**, **DNS**, **HTTPS**, **ICMP**)
- Wireshark (Protocol Analyzer)

<h3>Objectives</h3>

1. Create Windows 10 WM and Linux Ubuntu Server within Azure
2. Connect to Virtual Machine 1 Remote Desktop and download Wireshark
3. Ping WM 2's IP address to verify connectivity in CMD
4. Block WM 1's firewall in Azure and observe the closed traffic
5. Observe all traffic on ICMP, SSH, DNS, and RDP protocols

<h3>Actions and Observations</h3>
<p>

Installed Wireshark on WM1
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
 </p>
<br />
&emsp; 
&emsp;
<img src="https://imgur.com/QBbEbNt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Created a new inbound rule within Azure to ban all ICMP4 traffic.
 The image above is the inbound rule in motion. Used Ping to test connectivity and there were no replies from WM2. 


https://github.com/daltonsjones98
