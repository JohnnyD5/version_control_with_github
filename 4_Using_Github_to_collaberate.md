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
# 5. git merge
You made some changes on your local file, and some changes on github

To merge all changes:
```
git pull origin master
```

If there are conflicts:
1. solve the conflict
2. ```git commit```
3. ```git push```
