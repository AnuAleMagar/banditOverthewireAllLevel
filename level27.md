# level27

## Goal

There is a git repository at ssh://bandit27-git@localhost/home/bandit27-git/repo via the port 2220. The password for the user bandit27-git is the same as for the user bandit27.

## Solution
```
log in to bandit27
mktemp -d 
cd tempDir
cd clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
ls 
cd repo
ls 
cat README
```
