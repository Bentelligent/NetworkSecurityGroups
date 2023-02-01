<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create 2 VM's in Microsoft Azure and connect using Remote Desktop
- Download Wireshark for Windows 10
- Ping a public website on Wireshark  
- Ping the other VM to observe the traffic between the two

<h2>Actions and Observations</h2>

<p>
<img src="https://imgur.com/YbXa6Lv.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step, we create 2 Virtual Machines, one running Windows 10 and another running Ubuntu Server. We connect to the Windows 10 Virtual Machine in Remote Desktop. Once connected, we use a browser to download Wireshark for Windows.
</p>
<br />

<p>
<img src="https://imgur.com/XlxIcDg.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
To explain the download of Wireshark, it's a program to monitor and manage the traffic between the networks and possibly interrupt the traffic. To start, we can ping (through Command Line) a public site such as Google or Amazon. It'll read back and show us the speed at which the data is being transferred between the website and the Virtual Machine. Now, we could also ping the other VM through the public or private IP address to show the speed of the traffic between the 2. 
</p>
<br />

<p>
<img src="https://imgur.com/n1bZEaH.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Through Wireshark we are able to monitor the traffic of the networks and the speeds. As stated in the previous, we can ping between the 2 virtual machines and view the traffic speeds. But going back to VM's on Azure, we can pause the networking and interrupt the traffic. It'll keep pinging but on Command Line, it will continue to say "Request Timed Out". And since it's a continuous ping, it will keep timing out until the VM is resumed on Azure. 
</p>
<br />
