# level7

## Goal

Find password in data.txt file which is next to 
the word millionth

## Solution
```
ls
cat data.txt | grep 'millionth'
or
grep -owP '.{0,50}millionth.{0,50}' data.txt
;;here grep is used to search for pattern and print them 
;;{0,50} 0 represents the minimum number of preceding pattern and 50 represents maximum

