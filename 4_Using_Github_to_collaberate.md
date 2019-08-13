# 1. Syncing repositories
If you made changes on local folders and want to update github. Two ways:
1. Push through `Github Desktop` app
2. Use git bash
```
git push origin master
```

# 2. See remote repository
```
git remote -v
```
# 3. pulling changes
If you made changes on github and want to update local folders
```
git pull  
```

# 4. Add collaborator on Github
1. Go to project folder on Github
2. Go to settings
3. Click `collaborators`
4. Add github username
5. Click `Add collaborator` button

# 5. Git merge
You made some changes on your local file, and some changes on github

To merge all changes:
```
git pull origin master
```

If there are conflicts:
1. solve the conflict
2. use git add on conflicting files before committing
3. ```git commit```
4. ```git push```

# 6. Make a pull request
1. create a branch locally
```
git branch branch_name
```
2. check out the branch
```
git checkout branch_name
```
3. make changes to a file or files and make a commit
4. push the branch to your fork or github repository
```
git push origin `branch_name`
```
5. create a pull request from the branch into master or other's repository
6. wait for response if it is other's repository or commit merge if it's your own repository.  

# 7. Concept map
![pic5](pic/pic5.png)

# 8. About fork
Fork the repository and clone your fork
Now that you've learned how to fork a repository, push changes to your fork, and make a pull request, you’re ready to contribute to the create-your-own-adventure story that you saw at the beginning of the lesson. To do this, first you should fork this repository. Then clone your fork, and make a branch to make your changes in.

*Note*: You could make your changes directly to the master branch in your fork, but when contributing to a public repository, it’s standard practice to make the changes in a non-master branch within the fork. This way, you can easily keep your master branch up-to-date with master of the original repository, and merge changes from master into your branch when you are ready.

*Note for Windows Users*: The story has grown so large that it exceeds Windows' path length limit. If you encounter an error when cloning you can work around it by modifying a configuration setting. Run this command in git bash: `git config --system core.longpaths true`.

# 9. Syncing a fork
1. Clone the fork to local project
2. Fetch the branches from upstream repository
```
git fetch upstream
```
3. Checkout fork's local `master` branch
```
git checkout master
```
4. Merge the changes from upstream/master into your local master branch. This brings your fork's master branch into sync with the upstream repository, without losing your local changes.
```
git merge upstream/master
```
If your local branch didn't have any unique commits, Git will instead perform a "fast-forward".
