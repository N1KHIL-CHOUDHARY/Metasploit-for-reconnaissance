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
<img width="732" height="498" alt="494956916-f0b21e63-c196-4f8c-9cf4-c57bf565aa07" src="https://github.com/user-attachments/assets/5a0253bb-cf90-4e9e-9cf7-f1f52a8b9e44" />

Invoke msfconsole:
## OUTPUT:

<img width="728" height="444" alt="image" src="https://github.com/user-attachments/assets/687003f6-b404-4dea-acb3-e0f4808a026b" />


Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

<img width="895" height="633" alt="428283588-5c4cca07-ecfc-4a6d-868e-bb10583f3a08" src="https://github.com/user-attachments/assets/84bb24e1-aca0-4f99-82e0-33db6cf855e3" />


Port Scanning:
Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).

<img width="545" height="189" alt="Screenshot 2025-09-29 090716" src="https://github.com/user-attachments/assets/4f1ea003-e83a-4e71-8324-3b10ba1c12b9" />

use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.

msf > db_nmap 192.168.181.0/24

<img width="709" height="325" alt="image" src="https://github.com/user-attachments/assets/d7247197-2884-43d4-8fda-a6d2950eb558" />


Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to 

Metasploit's auxiliary modules and list all the scanner modules.

cd /usr/share /metasploit-framework/modules/auxiliary

kali > ls -l

<img width="746" height="454" alt="image" src="https://github.com/user-attachments/assets/869b8aa7-3117-493d-81e7-860283ab9a93" />


Search is a powerful command in Metasploit that you can use to find what you want to locate. 

msf >search name:Microsoft type:exploit

<img width="1707" height="411" alt="image" src="https://github.com/user-attachments/assets/a25d0579-0baf-4822-85f9-b529b1e20cfb" />


search type:auxiliary mysql

<img width="1415" height="451" alt="image" src="https://github.com/user-attachments/assets/5e59866a-af19-41be-bee5-1beb4d22665b" />

use 11

<img width="1199" height="376" alt="image" src="https://github.com/user-attachments/assets/1e0e3627-0fec-499a-954f-58a53346dc71" />


set RHOSTS <IP>

<img width="586" height="110" alt="image" src="https://github.com/user-attachments/assets/449a8dd5-7e3f-4f15-b4ed-d25d15a87903" />


use auxiliary/scanner/mysql/mysql_login

<img width="1400" height="543" alt="image" src="https://github.com/user-attachments/assets/4144f0e4-c087-4f96-a717-f58efbc09938" />



set PASS_FILE /usr/share/wordlists/rockyou.txt

set RHOSTS <metasploitable-ip-address>

set BLANK_PASSWORDS true

set verbose no

run

<img width="894" height="270" alt="image" src="https://github.com/user-attachments/assets/a61039b2-d609-4077-b659-cb811ced0f96" />

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully



