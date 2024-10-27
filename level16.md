# level16

## Goal

The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them.

## Solution
```
nmap -p 31000-32000 localhost
cat /etc/bandit_pass/bandit15 | openssl s_client -connect localhost:portnumber -ign_eof //here port number is replaced by the port that is open 
copy the ssh key
logout from level16
make a file with the ssh key
chmod 700 ssh.key
ssh -i ssh.key bandit17@bandit.labs.overthewire.org -p 2220
cat /etc/bandit_pass/bandit17 //to get the current password
```
