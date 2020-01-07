# Git
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.  Git is easy to learn and has a tiny footprint with lightning fast performance. It outclasses SCM tools like Subversion, CVS, Perforce, and ClearCase with features like cheap local branching, convenient staging areas, and multiple workflows.

## Configure in Windows

```
1.Download and Install git from :: https://git-scm.com/downloads
2.Setting Up git
  git config --global user.name "xxx"
  git config --global user.email xxx@yahoo.com
  git config --global color.ui true
  git config --global color.status auto
  git config --global color.branch auto
  
3.Create a repository in the Remote server: HTML

4.Clone the repository: 
  git clone https://github.com/maainul/HTML.git
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
Git Link
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

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

