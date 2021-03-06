# 1. What makes a repository a repository?
git repository stores lots of megadata of the history of the data and a hidden file `.git`

To show hidden files:
```
ls -a
```
# 2. Initializing a repository
## Git repositories and directories
Each Git repository is tied to a specific directory - the directory where you ran git init. Only files from that directory (and subdirectories inside that directory) will be contained in that repository, and you can have different repositories in different directories.

Note: it's often the case that a Git repository in some directory will only contain, or track, some of the files in that directory, rather than all of them. You'll see how this works later this lesson.
Go to a folder to set up a new repository
```
git init
```
Use git status to track status of files
```
git status
```
# 3. Staging area
![pic1](pic/pic1.png)
Add files to staging area
```
git add `filename`
```
# 4. commit message
## How to write a commit message
You're about to make your first commit to your reflections repository. When you do this, you'll need to write a commit message describing your changes. If you followed the instructions in the "Setting Up Your Workspace" video for your platform near the end of Lesson 1, the editor you chose will appear as soon as you run git commit and allow you to write a commit message. If you get an error message, you should try revisiting the instructions in Lesson 1 and make sure your text editor is set up properly.

You can also specify a commit message via the command line by running git commit -m "Commit message" instead of just git commit. It's still a good idea to get an editor set up, since this will make it easier to write long commit messages that fully describe the change.

## Commit message style
While commit message style varies from person to person, this [style guide](http://udacity.github.io/git-styleguide/) describes some common best practices when writing commit messages.
# 5. add file and commit procedures
0. make changes to the file
1. add file to staging area
```
git add `filename`
```
2. Check status
```
git status
```
3. make commit
```
git commit
```
4. write description in commit log
5. can use git log to check commit
```
git log
```
# 6. git diff
![pic2](pic/pic2.png)
# 7. git checkout
use git checkout commitID to checkout a previous commit
```
git checkout `commitID`
```
use git chekcout master to return to the master commit
```
git chekcout master
```
# 8. Branches
![pic3](pic/pic3.png)
# 9. Create new Branches
```
git branch `branchname`
```
switch to the branch
```
git checkout `branchname`
```
make changes
commit the changes
# 10. when to create branch
* when I want to create something different
* context switching
* master branch as the production quality branch that never breaks, always Works
* development branch where active work is taking place on your project
* experimental branch
* unique feature branch
* you can share experimental and unique feature branch in public with the understanding that this isn't production quality work just yet
* Branch is good to collaborate publicly and with yourself.
* Brach allows the ability to context switch and go back to where to fix the bug
* Use branch to keep things organized when working with others
# 11. Viewing the commit history
The full command Caroline types to see the visual representation of the commit
 ```
history is git log --graph --oneline master coins.
```
# 12. go to a commit and create a branch
```
git checkout `commitID`
```
```
git checkout -b new_branch_name
```
# 13. merge branch into master
```
git checkout master
```
```
git merge master branch_name
```
## delete branch label
```
git branch -d branch_name
```
# 14. merge conflict
Need manually solve the conflict
# 15. Concept map
![pic4](pic/pic4.png)
