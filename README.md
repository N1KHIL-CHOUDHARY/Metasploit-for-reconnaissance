# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:

Find out the ip address of the attackers system
## OUTPUT:


Invoke msfconsole:
## OUTPUT:

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.



Port Scanning:
Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).


use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.

msf > db_nmap 192.168.181.0/24


Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to 

Metasploit's auxiliary modules and list all the scanner modules.

cd /usr/share /metasploit-framework/modules/auxiliary

kali > ls -l


Search is a powerful command in Metasploit that you can use to find what you want to locate. 

msf >search name:Microsoft type:exploit


search type:auxiliary mysql


search type:auxiliary mysql


use 11


set RHOSTS <IP>


use auxiliary/scanner/mysql/mysql_login


set PASS_FILE /usr/share/wordlists/rockyou.txt

set RHOSTS <metasploitable-ip-address>

set BLANK_PASSWORDS true

set verbose no

run

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully



