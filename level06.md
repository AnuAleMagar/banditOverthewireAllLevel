# level6

## Goal

the password is somewhere in the server and the file is owned bytes
user bandit7
owned by group bandit6
and size 33bytes


## Solution
here >dev>null is used to remove standard error.
everything in >dev>null directory is deleted permanently
here 2 is for standard err type ,if it was 1 then it's for standard output
```
ls
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

