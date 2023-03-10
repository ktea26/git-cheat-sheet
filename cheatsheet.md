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


#### Pull Request (gh pr create --help)
Created using web portal
Between a base and a secondary branch in order to merge changes from secondary to the main branch. 
Needs an author and reviewer to approve the request.
Can be attached to an issue (Bug) while creating the bug or through commenting in the PR with the keyword "Close #N", N = id of the bug

#### Branch protection
allows for different rules on a specefic branch (main), helps to make terms and conditions.

#### Code Owners
a file created globally in the repo to define each owner of a specfic file pattern
Useful when a PR has many different file patterns (.js, .Net, doc/*)


#### Branching Strategies 
1. Trunk base development 
##### Developments are always made on the main branch (devs needs to be experts)
3. Git flow
##### Key branch : develop. Feature branches are created from this branch. Release branches used for release stabilisation too. At the end all is merged back to develop and main. (requires a lot of work) 
4. GitHub Flow
##### Simpler. Provides feature isolation. (adapted to continuous deployment)

#### Open Source / Inner Source model
create a fork 
fix bug / add feature on local repo created
create a PR with the original repo as a target

#### Ways to integrate
1. Merge (git merge)
##### git checkout main
##### git merge features/feature1
##### git commit
3. Squash merge (git merge --squash ) to clean up historial commits and combine them in one
##### git checkout main
##### git merge --squash features/1234-new-killing-feature
##### git commit
4. rebase (git rebase) (allows for a linear graph) to update feature branch and re-apply commits (chan ges the parents of commits)
##### git rebase

#### cherry picking
git cherry-pick <commitid> <commitid2>
