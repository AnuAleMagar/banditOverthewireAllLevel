#level14

##Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.


##Solution
```
cat /etc/bandit_pass/bandit14 // to get current password
cat /etc/bandit_pass/bandit14 | nc localhost 30000 // to send the password to localhost 
```