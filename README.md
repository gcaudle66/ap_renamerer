<body>
<h1>ap_renamerer</h1>
<p>Python app to bulk rename access points on IOS-XE 9800 platforms WLCs. This uses the same import CSV file format 
used by Cisco Prime Infrastructure.</p> 
<p>This script uses the NetMiko module package for connecting via SSH to a single WLC to rename APs.</p> 

<p><ul>Takes input from CSV file that
is placed in same directory as
the Script file</ul>
<ul>• MACs formatted to xxxx.xxxx.xxxx format</ul>
<ul>Formats CSV Data • AP Names to lowercase</ul>
<ul>• Prompts user for target WLC IP and Credentials to login</ul>
<ul>• Gathers current AP’s Name and Ethernet MAC</ul>
<ul>Connect to WLC via SSH and
gathers info on Registered APs</ul>
<ul>• Looks for matching MAC Addresses</ul>
<ul>• Displays any matches found and displays them for user</ul>
<ul>Compares info from CSV
and WLC</ul>
<ul>•For each match command is created “ap name {current name
from WLC} name {desired AP name from CSV}</ul>
<ul>Creates commands for
renaming Aps</ul>
<ul>Sends commands to WLC to
rename APs</ul>
<ul>•logfile is created in same directory as script</ul>
<ul>Displays results “ssh_session_logfile.txt”</ul>
</p>

<p>Detailed instructions are located in the file 
<h2>Running AP Rename Script.pdf</h2> located in this repo or on the Wiki page</p>



</body