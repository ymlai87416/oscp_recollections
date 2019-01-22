# Progress

## Public network

### Infrastructure

* DNS server?
10.11.1.220 -> master, cannot ls 
10.11.1.221 -> slave

### 10.11.1.5               alice
Done

Too simple and use metasploit to exploit SMB server
From profile, it does not have any function

### 10.11.1.7               pedro
Need pivoting
seem related to 13?
229 is asking for 7

### 10.11.1.8               phoneix
Done

Advance comment system. from profile there is a mail server
How to get email from smtp?

### 10.11.1.10              mike

Done

Another very easy system, 
But I don't have do any post exploitation

### 10.11.1.13/10.11.1.14   bob/bob2

Done

Get a low shell and use upnphost to get root, seems nothing
* Why it is requesting thing from 7?

### 10.11.1.22              barry

Done

Use openfuck to crack it

### 10.11.1.24(3 Viewing)   payday

Done

* have a capture.php to it is 248 -> 220 pcap, containing the following password
* 220: ftp: brett/ilovesecuritytoo

This is a CS-cart server, nothing special, but has pop3 

### 10.11.1.31              ralph

Done 

Get password and login mssql and do the trick.

### 10.11.1.35(3 Viewing)   pain

Done

* Able to get a reverse shell, but not privilege escalation
* Compile udev locally and upload to the machine to root

### 10.11.1.39(1 Viewing)   leftturn

Done
Otis service, easy to prone, nothing special

### 10.11.1.44              314159265/pi

Forum said, I need further info to exploit this machine.
This machine has 2 port open, 22 and 8000...

the hostname is 314159265

### 10.11.1.49/10.11.1.50(1 Viewing)    bathany/bathany2 -> alice

nmap not just for default port? also UDP?

### 10.11.1.71              alpha

SKIP

Seems I got the database password list, but I cannot login...
This is a shellshock demo machine, I think i will skip it

### 10.11.1.72              beta

DONE, mail, -> python normal shell -> root
I have exploit the mail vulnerability, but cannot get the shell

### 10.11.1.73              gamma

DONE
hostnmae: GAMMA
Have lot of attack surface, but I haven't try it yet.

https://forums.offensive-security.com/showthread.php?18253-73-Hotot-s-Take

### 10.11.1.75              bruce

Cannot find any attack surface yet.
What is IRC?

Not showing up in my init scan, what is it? only 3 thread and what is IRC?

### 10.11.1.115             tophat

Done

Using openfuck to do the thing
have mysql open-up

### 10.11.1.116(1 Viewing)  dotty

Done

Using LFI to hack it. Cuppa CMS

### 10.11.1.125(1 Viewing)  sherlock

DONE 
Can download file without exploit
Femietter ftp can traversal the whole system
Then minishare service on port 123. which need to be migrate as soon as possible???
Or the machine is being stolen by other student.

### 10.11.1.128             dj

DONE 
Using SQL injection to hack into UltraVNC

DONE

### 10.11.1.133             gh0st

https://forums.offensive-security.com/showthread.php?18173-133-Hotot-s-Take

Haven't try it yet

### 10.11.1.136(2 Viewing)  sufferance

Done
Samba for scout, SSH for crack in
Exim is a fucking rabbit holes
Priv esc using silly user script modify PATH variable

### 10.11.1.141            fc4

Done, viewing file and getting reverse shell using the same webmin exploit

### 10.11.1.145(1 Viewing)  helpdesk

DONE 

Use of metasploit to create a reverse shell to do everything.
Use ManageEngine Service Desktop plus exploit in ruby + msfvenon java/meterpreter/reverse_tcp

### 10.11.1.146             susie

DONE Using FTP exploit, get the root

### 10.11.1.173             tears

This cannot be reached, and no doc on forum yet.

### 10.11.1.202             oracle

DONE Compromised by openfuck

### 10.11.1.209             kraken

DONE Compromised by unprotected tomcat

### 10.11.1.217             hotline

DONE Compromised by elasticx, and root with nmap

### 10.11.1.218             observer

DONE, from 234 I have send it a poison page and return a shell.
Traffic to master is boring. master check IPC$ sometime but cannot get thinc.admin hash
only robert hash.
Watch the forum, people say that this host is working on something special, listen with wireshark.

220/221 Broadcast to ask for 218. Why???
218 ask for 220/221/234

### 10.11.1.219             edbmachine

Done, port knocking, no nmap, install knockd.

### 10.11.1.220             master

DONE, but I cannot log into thru remote desktop
In SysVol I got the password of slave.
I got a FTP password for this, and a attack vector is removed (easy)

Haven't try it yet

### 10.11.1.221             slave

DONE, get the password from master and slave give me the hash for thinc.admin.
You can control this machine via other machine...

Haven't try it yet

### 10.11.1.223             jeff
DONE

This machine is jeff and it has a friend
Haven't try it yet

### 10.11.1.226             joe

Done.
The tftp service is very unstable, and hence have to use metasploit
tcp_nonx cannot be listen by nc

### 10.11.1.227             jd
Done, simple metaspliot exploit but not report

I have hacked it

Able to login later

### 10.11.1.229(2 Viewing)  mail

** 229 broadcast to get 7?

Standalone hack Ralph
hacked and ceo ask jeff, malroy and nina to send report to Ralph (7).

Forget to get hMail password

Done

### 10.11.1.230(1 Viewing)  kevin

Get IT security
Cannot connect to IT network...
cannot cachedump, check if there is newer tools

Done

### 10.11.1.234(1 Viewing)  core

DONE 
Just use a tool and you can root it??

Done, root using perl and prev esc

has IT network access to ** hack IT computer

### 10.11.1.237/10.11.1.238(2 Viewing)  humble/humble2

Done, humble cracked by mounting davfs2
Get initial shell by exploiting mongoDB 2.2.3

### 10.11.1.247             cory

DONE

### 10.11.1.251             fw_it

DONE 

### 10.11.1.252             fw_dev

DONE 

### 10.11.1.253             tricia

## IT network

Not yet find a way to get into, post exploit every machine again to check for entries.

https://www.offensive-security.com/metasploit-unleashed/proxytunnels/
3proxy?
Teach you how to setup socks on network.

### 10.1.1.233

DONE. This is jeff

### 10.1.1.224

DONE, This is niky
There is a secrete drive that I cannot break into.

### 10.1.1.226

Only ftp open for the first enum. Seems lot of steps
* UDP port? and a windows host

### 10.1.1.230 (Public)
DONE

### 10.1.1.235 (nina)

DONE 
Only ftp show up, what is it for>?
??? Why nina connect to people, have to probe the network...
This is a browse exploit

### 10.1.1.236 (carrie)

DONE
This apache dont allow me to scan, it has mail/smtp/pop, ssh, ftp, and dns
not enum ftp and dns yet

### 10.1.1.246 (Sean)

DONE

This is a WP site, enum died at the middle
Seems vulnerable to php remote code attack.
Have ftp and ssh

### 10.1.1.247

Like 248, have only ftp and rdp open.
Port to 10.11.1.247 Cory... have dependency and clue

### 10.1.1.248  (Brett)

DONE 

Only ftp and remote desktop open
Seems this is an easy root.

### dev network



## Unknown network

### 10.1.1.1

There is a webconsole on this machine
open port FTP, SSH, WEB
web not enum yet