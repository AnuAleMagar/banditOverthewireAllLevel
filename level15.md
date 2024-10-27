#level15

##Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

##Solution
```
cat /etc/bandit_pass/bandit15 | openssl s_client -connect localhost:30001 -ign_eof 
or 
echo 'currentpassword' | openssl s_client -connect localhost:30001 -ign_eof 
```
-ign_eof ignores the end of file and continue reading,so the server can send aditional information 
