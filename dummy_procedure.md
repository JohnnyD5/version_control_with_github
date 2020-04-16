Here is the detailed procedures of using git and version control on Linux or Mac machine without help of the github desktop app
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
# Synchronize changes
## Uploads all local commits to github
```
git push origin master
```
## Downloads most recent contents and changes
```
git pull
```
