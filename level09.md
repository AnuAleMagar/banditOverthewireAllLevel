# level9

## Goal

password is inside data.txt file in few human readable strings followed by several '='

## Solution

here the strings extract all the human readable string from the data.txt and grep == filter the line having == sign 
```
strings data.txt |grep ==
or 
grep -a '=' data.txt |grep -a -oP '\=+\s*\w+'
```