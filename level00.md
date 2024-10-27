# Level 0

## Goal
Connect to the server using SSH.

## Solution
 
-Here ssh is secure shell that securely connects to the server
to connect to the server we have this format of command that is ssh username@domainName/hostname -p portname
ssh is a client side program that is responsible for connecting client to the remote server and the connection is done using cryptographic protocol
here we have user=bandit0 ,ip/hostname=bandit.labs.overthewire.org and port is 2220 here -p denotes flag for portnumber

` ssh bandit0@bandit.labs.overthewire.org -p 2220 `

-for the next level the goal is to read a password which is in readme file in home directory

-to see the list of files and directory of the current directory

```
ls 
cat readme
```
here cat is to concatenate or display the output of the file, here readme is the filename
you will get the password 

