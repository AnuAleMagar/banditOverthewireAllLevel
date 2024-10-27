#level28

##Goal

There is a git repository at ssh://bandit28-git@localhost/home/bandit28-git/repo via the port 2220. The password for the user bandit28-git is the same as for the user bandit28.

##Solution
```
mktemp -d 
cd tempDir
git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
cd repo
ls
cat README.md //we get nothing here
git log //to see the git commit history
git show commit-hash
```
