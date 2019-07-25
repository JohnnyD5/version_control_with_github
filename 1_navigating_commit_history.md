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
