# git-notes
These are the common git command I use every day

### Video Tutorial

Here a video showing you my approach to using github and git.

- [https://youtu.be/9rbARG6iXlo](https://youtu.be/9rbARG6iXlo)

#### git add --all
if you start adding new files to your folder. Git will not actually know that it need to track it. 'git add --all' will add all the files you just added so git knows to track it.

#### git commit -am [message]
This command will do 2 things at one time. It will add your files then also commit it with a message. Normally you would have to do a 'git add [filename]' then git commit -m [message]. This does both. One thing to note is this will not add untracked files.

#### git pull
This pulled in new code from your remote repository. When you are working with a team you will get updated code in your Github repo. To get that updated code you run 'git pull'

#### git push
This command pushes your new changes to the remote repo.

#### git merge
This command merges your code with another branch.

#### git stash
This is used to stash away code you might not want to commit but still want to keep for further experimenting. This will stash it away and remove it from your code.

#### git stash pop
This will add back your last stashed code and remove it from the stash list.

#### git stash list
Will show you a list of stashed code.

#### git checkout [branch name]
This is how you can move to different branches in your code.

#### git checkout -b [branch name]
This does 2 things. It creates a new branch and then moves you into that branch

#### git status
Show your current git status

#### git diff
Shows you the difference between the code you just wrote and what is currently in your repo.

### Merging branches

Here is my flow of I merge my branches into master. You always want the master branch to be the cleanest branch, so you want to do merge conflicts only in your current branch you are making changes in and then once everything is clean and in sync with master, then you merge your branch into master. This keep master very clean and with minimal bugs. Here is the process:

1. On your current branch. You want to pull in all new changes from the master branch.

  ```
  git pull origin
  ```

2. Fix any merge conflicts or issues after merging if you have any.

3. Move to the master branch

  ```
  git checkout master
  ```

4. Merge your new branch updates into master

  ```
  git merge [name of branch you are merging]
  ```
