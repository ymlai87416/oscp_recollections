# Password crack

## software

* john the ripper
dictionary + rules

* hashcat
dictionary + rules

## dictionary

A list of dictionaries:

john basic

* brute force

    john 127.0.0.1.pwdump
* dictionary
    
    john --wordlist=/usr/share/wordlist/rockyou.txt 127.0.0.1.pwdump

* dictionary + rule

    john --rules --wordlist=/usr/share/wordlist/rockyou.txt 127.0.0.1.pwdump

hashcat basic

The output file is at hashcat.potfile

* Directory
    * ./rules => contains rules

* dictionary

    hashcat -a 0 -m 400 example400.hash /usr/share/wordlist/rockyou.txt

* dictionary + rules

    hashcat -a 0 -m 400 example400.hash /usr/share/wordlist/rockyou.txt -R ./rules/best64.rule

*  brute force
    
    hashcat -a 3 -m 400 example400.hash ?a?a?a?a?a?a

## recover hash 

### Windows

Use fgdump to dump password

|ID  | Method| Hashcat type|
|----|-------|-------|
|1   | LM Hash| 3000 |
|2  |  NTLM Hash| 1000 |

### Linux

|ID  | Method| Hashcat type|
|----|-------|-------|
|1   | MD5| 500 |
|2a  | Blowfish (not in mainline glibc; added in some Linux distributions)| 3200 |
|5   | SHA-256 (since glibc 2.7)| 7400 | 
|6   | SHA-512 (since glibc 2.7)| 1800|