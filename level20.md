#level20

##Goal

There is a setuid binary in a homedirectory what we need to do is connect it with the port and send the current password from the port and then the program will give the next level password

##Solution
```
ls
// opened another terminal as bandit20 user
nc -l -p portnumber //here give portnumber a value
currentpassword // then give the current password in input
// then in another port run command given below
./suconnect portnumber //the same portnumber as in next terminal
```
then we will get the next password