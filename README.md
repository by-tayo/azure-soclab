# SIEM Simulation with Microsoft Azure + Honeypot

## ✍️ Objective

In this lab, I created a SIEM Simulation using Microsoft Azure Services to view a live attack of incoming traffic targeting the honeypot (Windows 10 VM). The Windows 10 VM is open to any ports making it easy for attackers to enter the vulnerable machine.

---

Created a list of Resources for the SOC Lab involving a Resource group to store Azure services such as Windows 10 VM, Virtual network, Log Analytics workspace, and Microsoft Sentinel.

After creating the list of resources, I then configured the Network security group to allow any ports in to see the amass of incoming traffic.

In the Windows 10 VM I created, (connection via RDP) I have configured the firewall settings to be set OFF.

I went to the Microsoft Sentinel services page, created a workspace, installed two Data connectors (Security Events via Legacy Agent and Windows Security Events via AMA), and created a data collection rule for my virtual machine to forward logs to the Log Analytics workspace.

Querying the Log Analytics workspace using KQL to view Security Events with certain filters to view logs within a time period.

Utilized GeoIP data to construct a Live Attack Map viewing live-traffic (24-hour period).

After I viewed the 24-hour period of the Live Attack Map, I waited till 48-hours to see more incoming traffic populating.

---

## Source
Josh Madakor, Youtuber in the cybersecurity/information technology field.
