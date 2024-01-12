<h1>SOC Automation Project (Home Lab) | Part 1</h1>


 ### [Video Demonstration](https://youtu.be/UJeXcJ59xvY)


<h2>Description</h2>
<b>In part 1 of this lab, I will be creating a diagram of our lab to practice the logical flow of data - also to act as a reference point for my lab later. I demonstrate my proficiency of setting up diagrams for processes like the Wazuh security tool and reinforce my knowledge on how SOC Analysts interact with this system, as well as the function of the resource. The written lab suppliments the lack of voice in this lab. I have only screen recorded for this part of the project.
</b>
<br />
<br />

<h2>Languages Used</h2>

- <b>draw.io</b>


<h2>Directions (Step-By-Step)</h2>
<b>
  1. Select Blank Diagram
  2. Select Icons for Internet, Computer and Router, label accordingly - label computer icon "Windows 10 Client Wazuh Agent"
  3. Duplicate computer icon for SOC Analyst, place adjacent, label accordingly
  4. Duplicate internet x3, label: North: "Shuffle", East: "TheHive", West: "Wazuh Manager", South: "Internet"
  5. Connect Windows 10 icon to Router using arrow, label "Send Events"
  6. Change arrow type to connection on right-hand side
  7. Connect Router to Internet
  8. Connect Internet to Wazuh Manager, label: "Receive Events"
  9. Connect Wazuh Manager to Shuffle using straight line, label: "Send alerts"
  10. Connect Shuffle to Internet, label: "Enrich IOCs"
  11. Connect Shuffle to TheHive, label: "Send Alerts"
  12. Connect Shuffle to Internet, label: "Send email" (be sure to distinguish this line from preexisting (#10)
  13. Connect Internet to SOC Analyst, label: "Send & Receive email"
  14. Connect SOC Analyst to Internet, label: "Send Response Action"
  15. Connect Internet to Shuffle (indicating data flowing back through internet to shuffle)
  16. Connect Shuffle to Wazuh Manager, label: "Send Response Action"
  17. Connect Wazuh Manager to Windows 10, label: "Perform Responsive Action"
  
</b>
<br />
<br />


<h2>1. Use simple logic chart as reference point for diagram</h2>

<p align="center">
<img src="https://i.imgur.com/XwQ9ncS.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>2. Blank Diagram</h2>
<p align="center">

<img src="https://i.imgur.com/fPSd5tD.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>3. Use Logic Chart - View Progression: Selecting Icons </h2>

<p align="center">
<img src="https://i.imgur.com/kRwjZay.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>4. Plotting First Lines & Labelling Accordingly</h2>

<p align="center">
<img src="https://i.imgur.com/qPHFJUb.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>5. Continue to add labels, verify logic, view progression: </h2>


<p align="center">
<img src="https://i.imgur.com/CoYQa8t.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>6. Complete Diagram</h2>


<p align="center">
<img src="https://i.imgur.com/sBW6lEs.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>7. Set internal network for Linux</h2>


<p align="center">
<img src="https://i.imgur.com/fTb4kSn.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>8. Set internal network for Windows</h2>


<p align="center">
<img src="https://i.imgur.com/sES8GAo.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>9. Set up Windows 10 Pro</h2>


<p align="center">
<img src="https://i.imgur.com/nFuj56x.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>10. Set static IP in Windows to 192.168.20.10</h2>


<p align="center">
<img src="https://i.imgur.com/PFdkv7U.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>11. Set static IP in Linux to 192.168.20.11 > set Netmask at 24</h2>


<p align="center">
<img src="https://i.imgur.com/VqTS7B3.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>12. Ping Linux from Windows to confirm both are connected | NOTE: if you try to ping from Linux at this point, it won't go through because the firewall is enabled for Windows. Don't disable as we need it running for Part 2, so just ping from Linux.</h2>
<p align="center">
<img src="https://i.imgur.com/35Zb42j.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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
