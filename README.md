# CS 579 Reverse Engineering at NMSU

## Summary
This repository holds my LAB reports on reverse engineering malware samples from "Practical Malware Analysis"

## System SetUp
1.How I set up my reverse engineering system, using system isolation and network isolation
- I installed a Virtual Machine (Oracle VM VirtualBox Manager) on my computer system running Linux OS to isolate malware(s) that I will be analyzing from interacting with the hardware of my actual computer system.
- Then, I installed a guest Operating System (Windows 10) into the Virtual Machine to enable me to run my reverse engineering tools that I will be using for this lab and also provide me with an isolated environment where I will be analyzing windows malware samples. 
- In addition, I set my Virtual Machine NIC card to host-only mode to ensure that my computer system is prevented from communicating with the Linux host.
- Lastly, took a snapshot of my virtual machine to save its current state for safety and easy reversal of the virtual machine to a clean state in case there is an unexpected changes to the virtual machine by a malware infection during an analysis, before starting to conduct analysis. 

2.Why I used isolation?

Setting up an environment that allows for analyzing an active malware to avoid causing damage to a computer system or network with malware infections is necessary and good practice, hence the reason why i used isolation is to avoid putting my computer or any other computers on the network at needless and unexpected risk during an analysis

3.Tools I installed on the victim machine for analysis and what their uses
- PeID : To use in confirming whether a file is packed or obfuscated
- Strings: A sysinternals program to use to shows the strings in a program
- PEView: To provide me with useful summary information about the portable executable(s), including compile time and imports
- Dependency Walker: For showing imports
