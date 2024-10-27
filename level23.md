#level23

##Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

NOTE 2: Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…

##Solution
```
cd /etc/cron.d
cat cronjob_bandit24
cat /usr/bin/cronjob_bandit24.sh
cat /usr/bin/cronjob_bandit23.sh
mktemp -d  //it generates a temorary directory
cd temporaryDirectory
touch script.sh
nano script.sh  // here i wrote same code as bandit23.sh but change myname variable to 'bandit24'
chmod +x script.sh
./script.sh
here we get /tmp/MytargetValueofBandit24SimilarToPreviousLevel
cat /tmp/MytargetValueofBandit24SimilarToPreviousLevel 
```
here at first i tried to make a script file in home directory but it didn't permit so i make a temporary file 

