//This is git starters commands

## connect email and username with git
git config --global user.email shahidbilal125@gmail.com
git config --global user.name SALLU00125

## initialize the folder as local master branch of git
git init  // initializes the folder as git repository
git add . // adds to file to be staged

## Roll back added changes
git checkout . // recent changes rolled back

## Compares the current_file with its backup saved in master branch
git status // checking the status of modified files

## History of commits
git log // logs of commits
git log -p -int(no_of_comits) // shows the selected no of commits only

##
git diff // compares the
git diff --staged // compares the staged to the last commited file

git checkout -f //roles file back to the last commit

git commit -a -m "Commit messages" // directly commit without staging

git rm --cached 'file name ' // the filename will be reverted back to before the staged filename

git branch // Lists all possible branches
git branch 'newBranchName' // new branch created
git checkout newBranchName // got into new branch
git checkout -b 'newbranch name //create and get into the new branch

git remote add origin 'https://repolink'
git remote // tells name of remote repo
git remote -v // tells link of remote repo

//SSH KEYS
ssh-keygen -t rsa -b 4096 -C  'emailID'
eval $(ssh-agent -s)
ssh-add ~/.ssh/id_rsa

git remote set-url origin git@github.com:SALLU00125/C-coding.git
// sets the repo sshLINK with key provided above to set origin as remote repo

git push -u origin master // pushes master to origin (git@github.com:SALLU00125/C-coding.git)  remote repo
