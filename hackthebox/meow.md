# Hack The Box – Meow

## Objective
Learn basic network enumeration and Telnet access.

## Tools Used
- nmap
- telnet
- Linux terminal

## Enumeration

Scan the target:

nmap -sC -sV <target-ip>

Result:
23/tcp open telnet

## Exploitation

Connect using telnet:

telnet <target-ip>

Login credentials discovered:
Username: root  
Password: (blank)

After login, retrieve the flag file.

## Skills Learned
- Port scanning
- Telnet access
- Basic service enumeration
