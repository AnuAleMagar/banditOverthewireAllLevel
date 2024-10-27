# level10

## Goal

the password is stored in base64 format in data.txt


## Solution
```
ls
base64 -d data.txt
```
here base64 is binary to text encoding scheme
here base64 command extract the base64 character which is then decoded by -d 