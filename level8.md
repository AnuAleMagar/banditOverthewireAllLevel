#level8

##Goal

to find the password where the line having password occurs only once

##Solution
;;-o print the matching part , sort sorts out alphabetically and uniq -u only prints uniqe line
```
ls
sort data.txt | uniq -u
or
grep -oE '\b\w+\b' data.txt | sort | uniq -u
```