# ap_renamerer
Python app to bulk rename access points on IOS-XE 9800 platforms WLCs. This uses the same import CSV file format 
used by Cisco Prime INfrastructure. 
This script used the NetMiko module package for connecting via SSH to a single WLC to rename APs. 

Takes input from CSV file that
is placed in same directory as
the Script file
• MACs formatted to xxxx.xxxx.xxxx format
Formats CSV Data • AP Names to lowercase
• Prompts user for target WLC IP and Credentials to login
• Gathers current AP’s Name and Ethernet MAC
Connect to WLC via SSH and
gathers info on Registered APs
• Looks for matching MAC Addresses
• Displays any matches found and displays them for user
Compares info from CSV
and WLC
•For each match command is created “ap name {current name
from WLC} name {desired AP name from CSV}
Creates commands for
renaming Aps
Sends commands to WLC to
rename APs
•logfile is created in same directory as script
Displays results “ssh_session_logfile.txt”
