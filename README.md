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

# Git REAL
##                          Level 1
```
git help config
```
```
### 2.Starting a Repo
```
mkdir store
cd store
git init
```
### 3.Add file to staging area
```
git add READMe.txt
git status (To check whats changed since last commit)
```
### 4.Commit changes
```
git commit -m "Creat a README."
git status
```
### 5.Add both files to staging area 
```
git add README.txt LISENCE or git add --all (Add all new or modified file)
git status 
git commit -m "Add LICENSE and finish READ."
```
### 6.Git Timeline History
```
git log ()
git status
```
### 7.Different ways to add 
```
git add <list of files> (Add list of files)
git add --all (Add all files)
git add *.txt (Add all text files in current directory)
git add docs/*.txt (Add all txt files in docs directory)
git add docs/ (Add all files in docs directory)
git add "*.txt" (Add all txt files in the whole project)

```

### 9.Upload Repository
```
Create folder in your local server and type
git add REPOSITORY NAME
git status
git push origin master
git status
git log
```
