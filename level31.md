#level31

##Goal

There is a git repository at ssh://bandit31-git@localhost/home/bandit31-git/repo via the port 2220. The password for the user bandit31-git is the same as for the user bandit31.

Clone the repository and find the password for the next level.

##Solution
```
mktemp -d
cd tempDir
git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo
cd repo
ls
cat README.md
touch key.txt
vim key.txt //add May I come in?
git add . //here the file is not staged due to gitignore file 
git add -f key.txt
git commit -m""
git push origin master

```
here in this level we need to push a file named key.txt to the github repo 


