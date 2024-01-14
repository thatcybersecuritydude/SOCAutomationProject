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

- <b>1. Select Blank Diagram</b> 
- <b>2. Select Icons for Internet, Computer and Router, label accordingly - label computer icon "Windows 10 Client Wazuh Agent"</b>
- <b>3. Duplicate computer icon for SOC Analyst, place adjacent, label accordingly</b>
- <b>4. Duplicate internet x3, label: North: "Shuffle", East: "TheHive", West: "Wazuh Manager", South: "Internet"</b>
- <b>5. Connect Windows 10 icon to Router using arrow, label "Send Events"</b>
- <b>6. Change arrow type to connection on right-hand side</b>
- <b>7. Connect Router to Internet</b>
- <b>8. Connect Internet to Wazuh Manager, label: "Receive Events"</b>
- <b>9. Connect Wazuh Manager to Shuffle using straight line, label: "Send alerts"</b>
- <b>10. Connect Shuffle to Internet, label: "Enrich IOCs"</b>
- <b>11. Connect Shuffle to TheHive, label: "Send Alerts"</b>
- <b>12. Connect Shuffle to Internet, label: "Send email" (be sure to distinguish this line from preexisting (#10)</b>
- <b>13. Connect Internet to SOC Analyst, label: "Send & Receive email"</b>
- <b>14. Connect SOC Analyst to Internet, label: "Send Response Action"</b>
- <b>15. Connect Internet to Shuffle (indicating data flowing back through internet to shuffle)</b>
- <b>16. Connect Shuffle to Wazuh Manager, label: "Send Response Action"</b>
- <b>17. Connect Wazuh Manager to Windows 10, label: "Perform Responsive Action"</b>
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

<h2>3. Use Logic Chart - View Progression: Selecting Icons: </h2>

<p align="center">
<img src="https://i.imgur.com/kRwjZay.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>4. Plotting First Lines & Labelling Accordingly:</h2>

<p align="center">
<img src="https://i.imgur.com/qPHFJUb.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>5. Continue to add labels, verify logic, view progression: </h2>


<p align="center">
<img src="https://i.imgur.com/CoYQa8t.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>6. Complete Diagram:</h2>


<p align="center">
<img src="https://i.imgur.com/sBW6lEs.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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
