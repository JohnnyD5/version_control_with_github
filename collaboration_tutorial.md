# Tutorial of working with existing remote repository
## Create local repository
1. Navigate to the desired online/remote repository
2. Click `Code`
3. Copy the url
4. In local folder, open `Git Bash`
5. Type `Git clone` and then paste the url
6. Press Enter
## Sync with the remote repository master branch
1. in local repository, type `git brach -a`  # this is to check the master branch name
2. Location line: `remotes/origin/Head ->` and note whatever is after `origin/`. 
3. If it's main then `git pull origin main`, or if it's master then `git pull origin master`
## Pull request
1. `git pull origin main` # to sync and update local repository
2. create a new branch by typing `git checkout -b side_branch_name`
3. make whatever changes 
4. `git status` to check the status, note the status message hints about what to do next
5. 
