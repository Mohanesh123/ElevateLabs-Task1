🛡️ Cybersecurity Internship - Task 1: Port Scanning
🎯 Objective
To perform basic network reconnaissance using Nmap in a controlled environment (Kali Linux VM) to identify open ports on devices within the local network segment.\n

🛠 Tools Used
.Kali Linux (Virtual Machine)
.Nmap
.Wireshark
.VirtualBox
⚙️ Setup
Installed VirtualBox from the official website.
Set up a Kali Linux virtual machine .
Used Kali's pre-installed tools: nmap, ifconfig, and wireshark.
🧪 Methodology
1.Started Kali Linux in VirtualBox.Checked IP address of the Kali machine using:
bash



ifconfig
2.Launched Wireshark in the background to capture packets during the scan:
bash


wireshark 
3.Ran a TCP SYN scan on the local subnet:
bash


nmap -sS 10.0.2.0/24 -oN scan_results.txt
4.This scanned all IPs in the range 10.0.2.1 to 10.0.2.255.
5.Saved results to a text file (scan_results.txt) for submission.
6.Analyzed captured packets in Wireshark , filtering by tcp to observe Nmap's SYN packets and responses from target hosts.
