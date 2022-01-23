### #Git commands :





**#Getting and creating projects**

| `git init`   | initialize new git repository on your local machine          |
| ------------ | ------------------------------------------------------------ |
| `git clone ` | clone a remote repository to your local machine using Https or Ssh |



**#Basic snapshotting**

| command                           | description                                   |
| --------------------------------- | --------------------------------------------- |
| `git status`                      | check status                                  |
| `git add [filename.txt]`          | add a File to a staging area                  |
| `git add -A`                      | add all new and staged files to staging  area |
| `git commit -m`"[commit message]" | commit changes                                |
| `git rm -r [filename.txt]`        | remove a file or a folder                     |

**#Branching and merging**

| commands                                             | description                                             |
| ---------------------------------------------------- | ------------------------------------------------------- |
| `git branch`                                         | list branches (the asterisk denotes the current branch) |
| `git branches -a`                                    | list all branches (local and remote)                    |
| `git branch [branch_name]`                           | create a new branch                                     |
| `git branch -d [branch_name]`                        | delete a branch                                         |
| `git push origin --delete [branch_name]`             | delete a remote branch                                  |
| `git checkout -b [branch_name]`                      | create a branch and switch to it                        |
| `git checkout -b [branch name] origin/[branch name]` | clone a remote branch and switch to it                  |
| `git branch -m [old branch_name]`[new branch_name]   | rename a local branch                                   |
| `git checkout [branch_name]`                         | switch to a branch                                      |
| `git checkout -`                                     | switch to the branch last checked out                   |
| `git checkout -- [file_name.txt]`                    | discard changes to a file                               |
| `git merge [branch_name]`                            | merge a branch to the active branch                     |
| `git merge [source branch] [target branch]`          | Merge a branch into a target branch                     |
| `git stash`                                          | Stash changes in a dirty working directory              |
| `git stash clear`                                    | Remove all stashed entries                              |



**#Sharing and updating Projects**

| commands                                                     | description                                                 |
| ------------------------------------------------------------ | ----------------------------------------------------------- |
| `git push origin [branch name]`                              | Push a branch to your remote repository                     |
| `git push -u origin [branch name]`                           | Push changes to remote repository (and remember the branch) |
| `git push`                                                   | Push changes to a remote repository                         |
| `git push origin --delete [branch name]`                     | delete a remote branch                                      |
| `git pull`                                                   | Update local repository to the newest commit                |
| `git pull origin [branch name]`                              | Pull changes from remote repository                         |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add  a remote repository                                    |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH                     |

**#Inspecting and comparing**



| commands                                   | description                    |
| ------------------------------------------ | ------------------------------ |
| `git log`                                  | view changes                   |
| `git log --summary`                        | view changes (detailed)        |
| `git log --oneline`                        | View changes (briefly)         |
| `git diff [source branch] [target branch]` | Preview changes before merging |

