Here is the detailed procedures of using git and version control on Linux or Mac machine without help of the github desktop app
# How to copy a repository to a new repository
1. Clone repository to a folder
```
cd existing-project
```
open here a git terminal
git remote set-url origin <NEW_GIT_REPO>
git push -u origin --all
git push origin --tags
# Create a repository
1. Go to my github
2. Under the repository name, copy HTTPS url.
3. open terminal and go to current working directory where you want the cloned directory to be made
4. `git clone` url, e.g.
```
git clone https://github.com/JohnnyD5/python_cheat_sheet.git
```
5. Check repository history
```
git log
```
**Comments:** Using `git clone` copies all git history of the file besides the contents. Using `Download` only saves contents of the file without any git structure.

# Make file and edit
**Comments:** You need to add new file into the git structure before you can use version control on it.
1. Make file  
```
echo "contents" > filename.extension
```
2. Add file to git structure   
```
git add filename.extension
```
3. check file status
```
git status
```
4. Use atom to edit and commit  
or Use
```
git commit -m "commit message"
```
5. To delete a file
```
git rm filename.extension
```
**Comments:** Sync every time you make changes and commits!
# Synchronize changes
**Comments:** Here we don't use branch, we make changes directly to origin master. See detailed guide on branch to have better understanding.
## Uploads all local commits to github
```
git push origin master
```
** Comments:** The system asks for the credentials of github account.
## Downloads most recent contents and changes
```
git pull
```
** Comments:** If you make changes online, just git pull. It automatically syncs with newest online version. No credentials needed.
