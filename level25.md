# level25

## Goal

Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.



## Solution
```
ls
cat /etc/passwd |grep bandit26 
cat /usr/bin/showtext
exit from bandit25
scp -P 2220 bandit25@bandit.labs.overthewire.org:bandit26.sshkey . //to securely copy to the localmachines
chmod 700 bandit26.sshkey
make the terminal as small as possible
ssh -i bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220
:set shell?
:set shell=/bin/bash
:shell
ls
cat /etc/bandit_pass/bandit26
```

