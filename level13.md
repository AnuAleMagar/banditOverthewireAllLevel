# level13

## Goal

The password for the next level is stored in /etc/bandit_pass/bandit14 and can
only be read by user bandit14.
For this level, you don’t get the next password,
but you get a private SSH key that can be used to log into the next level.
Note: localhost is a hostname that refers to the machine you are working on

## Solution
scp -P <port> <user>@<IP>:<remotefilepath> <localfilepath> it securly copy the content of hostserver to localmachines

ssh -i filename user@host -p portnumber it connects to the host server using ssh private ke

```
sshkey.private
exited from lab 13
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private .
chmod 700 sshkey.private // change the mode to read write and execute to me only
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
```
