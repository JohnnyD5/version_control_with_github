# 1. Version Control
Git: version control system
Github: code sharing and collaboration platform

## Comparing two files
On windows: 
`FC oldfile  newfile`
On Mac or Linux:
`diff -u oldfile newfile`

You can change windows prompt to linux style by using git bash
Download git from git website
# 2. when to save
As a programmer, when would you want to have a version of your code saved?
* when you choose to save a version
# 3. How Often to Commit
Since you can choose when to make a commit, you might be wondering how often to commit your changes. It's usually a good idea to keep commits small. As the diff between two versions gets bigger, it gets harder to understand and less useful. However, you don’t want to make your commits too small either. If you always save a commit every time you change a line of code, your history will be harder to read since it will have a huge number of commits over a short time period.

A good rule of thumb is to make one commit per logical change. For example, if you fixed a typo, then fixed a bug in a separate part of the file, you should use one commit for each change since they are logically separate. If you do this, each commit will have one purpose that can be easily understood. Git allows you to write a short message explaining what was changed in each commit, and that message will be more useful if each commit has a single logical change.
# 4. 
## It is important to know how to open text editor from either windows or linux machine
**Atom** 

On windows, in git terminal type in  
`echo 'alias atom="C:/Users/zding5/AppData/local/atom/atom.exe"' >> ~/.bashrc`

then type `atom` to open program on windows
# 5. Install git
to check git version:  
`git --version`
# 6. Cloning and exploring the repo
<https://www.youtube.com/watch?time_continue=118&v=WQjNhypqwNE>
## Cloning a Repository
To clone a repository, run `git clone` **followed by a space and the repository URL**.

## Asteroids URL
Use the following url to clone the Asteroids repository: <https://github.com/udacity/asteroids.git>

## Exiting `git log`
To stop viewing git log output, press `q` (which stands for quit).

## Getting Colored Output
To get colored diff output, run `git config --global color.ui auto`

## Copying and Pasting from the Command Line
To complete this quiz, you'll want to copy and paste some commit ids.

### Windows
The default way to copy/paste in Git Bash is by using the menu (accessed by going to the top left) to "mark" to select what you want to copy and then use the menu again to paste.

This gets inefficient pretty quickly, so it's a good idea to set up QuickEdit mode to make copying and pasting much faster.  To do this, go to `Menu->Properties` and in the `Options` tab select `QuickEdit` Mode.

Then you can copy text by selecting it and then right clicking, and you can paste by right clicking without anything selected on the screen.

Those instructions are for the Command Prompt program, but they will also work for Git Bash
### Mac
To copy and paste within the terminal on Mac, use `Cmd+C` and `Cmd+V`

### Ubuntu
To copy and paste within the terminal on Ubuntu, use `Ctrl+Shift+C` and `Ctrl+Shift+V`.

## Using `git log` and `git diff`
As a reminder, running `git log` will show a list of the recent commits with information about them, including commit IDs. Running `git diff` followed by two commit IDs will compare the two versions of the code in those commits. 
# 7. Git Errors and Warnings Solution
## Should not be doing an octopus
Octopus is a strategy Git uses to combine many different versions of code together. This message can appear if you try to use this strategy in an inappropriate situation.

## You are in 'detached HEAD' state
HEAD is what Git calls the commit you are currently on. You can “detach” the HEAD by switching to a previous commit, which we’ll see in the next video. Despite what it sounds like, it’s actually not a bad thing to detach the HEAD. Git just warns you so that you’ll realize you’re doing it.

## Panic! (the 'impossible' happened)
This is a real error message, but it’s not output by Git. Instead it’s output by GHC, the compiler for a programming language called Haskell. It’s reserved for particularly surprising errors!

**Takeaway** We hope these errors and warnings amused you as much as they amused us! Now that you know what kind of errors Git can throw, you’re ready to start checking out previous versions of files with Caroline.

# 8. Git Checkout
<https://www.youtube.com/watch?v=enodgfNvUsc>

We can temporarily change our files back tto how they were at the time of any commit. This is called a git checkout. It's like restoring a previous version.

In git, checking out a commit means resetting all of your files to how they were at the time that commit was made.

## why checkout out a previous version?
If a bug was introduced, but you're not sure which commit introduced it, you can test whether a commit has the bug by checking out that commit and running the code

## walkthrough
for the asteroids folder
```
git log > gitlog.txt
```
We think the Revert Control was a working commit. So check out the commit
```
git checkout b0678b161fcf74467ed3a63110557e3d6229cfa6
```
`b0678b161fcf74467ed3a63110557e3d6229cfa6` is the commit ID

Now you can go to the html file to see what happens

You can still get back to the most recent commit by typing git checkout followed by its ID

But what if you don't remember the ID?

In next md file, you'll learn another way to switch between commits without knowing their IDs


