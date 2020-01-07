# Git
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.  Git is easy to learn and has a tiny footprint with lightning fast performance. It outclasses SCM tools like Subversion, CVS, Perforce, and ClearCase with features like cheap local branching, convenient staging areas, and multiple workflows.

# Git Link
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
# Configure Git: 
## Configure in Windows

```
Download and Install git from :: https://git-scm.com/downloads
Setting Up git
  git config --global user.name "xxx"
  git config --global user.email xxx@yahoo.com
  git config --global color.ui true
  git config --global color.status auto
  git config --global color.branch auto
```
## Installing git on Linux
```
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git-core
```
For Ubuntu, this PPA provides the latest stable upstream Git version
```
sudo add-apt-repository ppa:git-core/ppa
sudo apt update; apt install git
```

# Move Operation: (Move file to another directory)

```
pwd
ls
mkdir src
git mv string.c src/
git status -s
git commit -m "Modified directroy"
git push origin master
```
# Rename Operation: (Rename file)

```
pwd
ls
cd src
git add makefile
git mv string.c string_operations.c
git status -s
git commit -a -m "added makefile and rename file string.c to string_operations.c"
git push origin master
```

# Delete Operation: (Delete file from repository)

```
pwd
ls
cd src
git log
git rm string_operations.c
git status -s
git commit -a "delete string_operations.c"
git push origin master
```
# Fix Mistake Operation: 
## Mistake 1 : Delete from local repository
### Suppose you delete a file from your local repository and you want your file back

```
# Check your file first.
pwd
git status -s
git checkout
git checkout string_operations.c
git status -s

## if found run file back operation

ls -1
rm string_operations.c (file back operation)
ls -1
git status -s
git checkout string_operatios.c
ls -1
git status -s
```
# Stash Operation: 

```
git status -s
git stash
git status -s
git stash list
git status -s
git stash pop
```
# Tag Operations: Give meaningful name to a specific version
## Create Tag:
```
pwd
git tag -a 'Release 1_0' -m 'Tag basic string operations code' HEEAD
git push origin master

```
## View Tag:
```
git pull origin master
git tag -l
git show Release_1_0
```
## Delete Tag:
```
git tag
git tag -d Release_1_0
git push origin master
```
