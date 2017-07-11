# git-notes
These are the common git command I use every day

- git add --all
- git commit -am [message]
- git pull
- git push
- git merge
- git stash
- git checkout
- git checkout -b [branch name]
- git status
- git diff

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
