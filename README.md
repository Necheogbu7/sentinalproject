<h1>Failed RDP to IP Geolocation Information</h1>


 ### YouTube Demonstration 
 -[walkthrough](https://youtu.be/OO8kANl7fcw?si=1ElNgIhF50IsvH5G)


<h2>Description</h2>
<b>The Powershell script used in  repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third-party API to collect geographic information about the attackers' location.
</b>
<br />
<br />
The script is used in this demo where I set up Azure Sentinel (SIEM) and connect it to a live virtual machine that i made vunerable by turning off firewall and allowing all ports  acting as a honey pot.
We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to
Look up the attackers' Geolocation information and plot it on an Azure Sentinel Map!
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/TmEMcM5.jpg"(https://ibb.co/nmNwBZV)" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 
- <b>Kql:</b>used to query the event logs in log analytics  
<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from ukraine coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://i.ibb.co/kBsGJkr/Screenshot-2024-09-10-104511.png" alt="Screenshot-2024-09-10-104511" height="85%" width="85%" />
</p>

<h2>World map of incoming attacks after 30 min  (built custom logs including geodata)</h2>

<p align="center">
<b><img src="https://i.ibb.co/zVWgK91/Screenshot-2024-09-10-101844.png" alt="Screenshot-2024-09-10-101844" height="95%" width="95%" /></b>
</p>
<h2>World map of incoming attacks after 1 hour   (built custom logs including geodata)</h2>

<p align="center">
<b><img src="https://i.ibb.co/bgpFK8Q/Screenshot-2024-09-10-103650.png" alt="Screenshot-2024-09-10-103650" height="95%" width="95%" /></b
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
