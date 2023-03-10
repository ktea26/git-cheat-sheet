# My Git CheatSheet
## Create a repo: 
##### git init   
#### Initializes an empty Git repository in the folder we are in '~/src/gitcheatsheet/.git/'
##### git clone
#### Copies an existing repo 
##### git status
#### Gives the status of the repository: pending changes, possible actions, etc.

##### git log  
Indicates the the history of commits in the current branch and returns the HEAD which points to the branch on which we are

##### git checkout -b new-branch-name
Creates anew branch, and moves there

#### git branch -d branch-name
Deletes the branch

#### git branch
Shows the list of branches


#### git remote -v
to get all remotes 

#### git remote set-url origin new-url-link
Changes remote URL 

#### git push
Pushes changes on local repo to remote repo, but local repo needs to be updated first using fetch & pull

#### git fetch 
Shows the updates of the default remote repository

#### git pull
Applies the updates from remote to local repo
