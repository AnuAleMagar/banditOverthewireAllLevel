#level29

##Goal

There is a git repository at ssh://bandit29-git@localhost/home/bandit29-git/repo via the port 2220. The password for the user bandit29-git is the same as for the user bandit29.

Clone the repository and find the password for the next level.

##Solution

```
mktemp -d
cd tempDir
git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo
git branch -a
git checkout remotes/origin/dev
git log
git show commit-hash
```
