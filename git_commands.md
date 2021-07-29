

![MSS logo](Images/MSS.png "MSS logo")
  <span style="color:red"> _CREATED BY MSS_ </span>

#  ***THE GIT STARTER GUIDE***


## What is the behind scheme?

<p>&nbsp;</p>

  ![diagram ](Images/lifecycle.png "Lifecycle")
  ____________________

## Connect email and username with git
  <p>&nbsp;</p>

  git config --global user.email shahidbilal125@gmail.com

    >Connects email int git

  git config --global user.name SALLU00125

    >connects user name into git
  ____________________
## Initialize the folder as local master branch of git

  <p>&nbsp;</p>

  git init

    >initializes the folder as git repository
  ____________________
## STAGING (_file in intermediate process in finalization_)

  <p>&nbsp;</p>

  git add .

    >adds to file to be staged

  ____________________
## Roll back added changes

  <p>&nbsp;</p>

  git checkout .

    >recent changes rolled back
  ____________________
## Compares the current_file with its backup saved in master branch

<p>&nbsp;</p>

  git status

    >checking the status of modified files
  ____________________
## History of commits  

  <p>&nbsp;</p>

  git log

    > logs of commits

  git log -p -NoOfCommits

    >shows the selected no of commits only
  ____________________
## Git comparative commands  

  <p>&nbsp;</p>

  git diff

    >compares working directory to staging files (ADD) and used after git status

  git diff --staged

    >compares the staged to the last commited file

  ____________________
## Rollback the change made

<p>&nbsp;</p>

  git checkout -f

    >roles staged file back to the last commit
  ____________________
## commit without staging

<p>&nbsp;</p>

  git commit -a -m "Commit messages"

    >directly commit without staging
  ____________________
## Removes file from the staging area and hence file is not in git tracking anymore

<p>&nbsp;</p>

  git rm --cached 'file name '

    >the filename will be reverted back to before the staged filename
  ____________________
# ___BRANCHES IMPORTANT___

  ##  *every branch is just a repo copy*
  #### _Main copy is master_

<p>&nbsp;</p>

  git branch

    >Lists all possible branches

  git branch 'newBranchName'

    >new branch created

  git checkout newBranchName

    >got into new branch

  git checkout -b 'newbranch name

    >create and get into the new branch
  ____________________    

# Making variable Origin

### _that contains SSH address of the repo_
###  origin var is named for ease

<p>&nbsp;</p>

  git remote add origin https://repolink

    >http will not work SSH is below

  git remote

    > view name of remote repo

  git remote -v

    > view link of remote repo
  ____________________

# Making RSA KEYS FOR encrypt decrpyt

  ### use them as it is and read more about them on github docs

  #### keys are stored by default in users/.ssh ,copy paste them in save folder



<p>&nbsp;</p>

___SSH KEYS___

-ssh-keygen -t rsa -b 4096 -C  'emailID'

    >gnerate key

eval $(ssh-agent -s)

    >paste as it is

ssh-add ~/.ssh/

    > paste as it is

git remote set-url origin git@github.com:SALLU00125/C-coding.git

    >sets the repo's ssh LINK in origin variable

    >This repo is remote repo

  ____________________

# Pushing the local repo to remote repo on GIT
<p>&nbsp;</p>

git push -u origin master

    > pushes master to origin (git@github.com:SALLU00125/C-coding.git)  remote repo
