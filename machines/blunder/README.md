Full write-up coming soon(tm) :)

# Commands
## enumeration
nmap -Pn -n -vvv -oN nmap-initial 10.10.10.191 

## apache enumeration
gobuster dir -u http://10.10.10.191 -w /usr/share/wordlists/dirb/common.txt -o gobust.out -x txt,html,php

## making custom wordlists
cewl 10.10.10.191 > blunder-wordlist.txt

# Further reading and links
Bludit Brute Force Mitigation Bypass: https://rastating.github.io/bludit-brute-force-mitigation-bypass/
Bludit password generation source code: https://raw.githubusercontent.com/bludit/password-recovery-tool/master/recovery.php
Sudo exploit >= 1.8.28: https://www.exploit-db.com/exploits/47502
