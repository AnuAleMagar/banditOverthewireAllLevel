#level21

##Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.


##Solution
```
cd /etc/cron.d
ls
cat cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/randomnumber //it is given by the file cronjob_bandit22.sh

