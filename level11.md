#level11

##Goal

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

##Solution
```

tr 'A-Za-z' 'N-ZA-Mn-za-m' <data.txt
```
here tr denotes translation
'A-Za-z' means all upper and lower case
'N-ZA-Mn-za-m' it means ROT13 and <data.txt gives the data to be translated to the command