git config --global user.email shahidbilal125@gmail.com
git config --global user.name SALLU00125

git init  // initializes the folder as git repository
git add . // adds to file to be staged

git checkout . // recent changes rolled back

git status // checking the status of modified files

git log // logs of commits

git log -p -int(no_of_comits) // shows the selected no of commits only

git diff // compares the
git diff --staged // compares the staged to the last commited file

git checkout -f //roles file back to the last commit

git commit -a -m "Commit messages" // directly commit without staging

git rm --cached 'filename.extension' // filename.extension would be removed from staging already

touch .gitignore // untracked file is put in this file
                // .gitignore -> *.extension " ignores all these extensions"


git branch 'newBranchName' // new branch created
git branch                // checks the available branches
git checkout 'newBranchName' // swithced to new branch
