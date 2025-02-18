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
<img width="952" alt="Screenshot configuring firewall to stop ping traffic" src="https://github.com/user-attachments/assets/ff4597e5-bb88-4153-ba75-c1229b84b378" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img width="949" alt="Screenshot configuring firewall to stop ping traffic png2" src="https://github.com/user-attachments/assets/d87aa1d4-6290-43dd-a78d-13aede2bc8b4" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img width="952" alt="Screenshot configuring firewall to stop ping traffic png3" src="https://github.com/user-attachments/assets/f5bc798b-2e31-4356-8b75-34852cc2d852" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
