#level5

##Goal

The password is inside the file which has following propertise
human-readable
1033 bytes in size
not executable

##Solution
```
ls
cd inhere
ls
find ./ -type f -size 1033c ! -executable //here above command search for the file that is not executable and with size 1033c
cat ./maybehere07/.file2
```
