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

1. Initiate a perpetual/non-stop ping from your Windows 10 VM to your Ubuntu VM
-   Open the Network Security Group your Ubuntu VM is using and disable incoming (inbound) ICMP traffic
-   Back in the Windows 10 VM, observe the ICMP traffic in WireShark and the command line Ping activity
-   Re-enable ICMP traffic for the Network Security Group your Ubuntu VM is
-   Back in the Windows 10 VM, observe the ICMP traffic in WireShark and the command line Ping activity (should start working)
-   Stop the ping activity

<h2>Actions and Observations</h2>

<p>
<img width="952" alt="Screenshot configuring firewall to stop ping traffic png3" src="https://github.com/user-attachments/assets/5c0ab3af-b94a-4746-9caf-d3885adc11f9" />

</p>
<p>
In this screenshot, we’re inside the Network Security Group (NSG) settings, specifically in the Inbound security rules section. You can see that an ICMP rule has been set to Deny, which blocks incoming ping requests to enhance security.
</p>
<br />

<p>
<img width="954" alt="Screenshot configuring firewall to stop ping traffic png4" src="https://github.com/user-attachments/assets/20d3a3cf-e29c-4a15-b14e-5d6d679c7cda" />

</p>
<p>In this screenshot, we're monitoring ICMP traffic on the Windows 10 VM using Wireshark and the command line. You can see the Ping requests and responses, helping us verify if the ICMP traffic is allowed or blocked.
</p>
<br />

<p>
<img width="948" alt="Screenshot of pinging virutal machines in microsoft azure " src="https://github.com/user-attachments/assets/99be791c-2a08-4cc6-90e5-3359dc9a218b" />



</p>
<p>
In this screenshot, we're checking ICMP traffic on the Windows 10 VM using Wireshark and the command line. The Ping activity should now be working, showing successful requests and responses.
</p>
<br />
