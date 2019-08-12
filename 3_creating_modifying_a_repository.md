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
![pic1](pic1.png)
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
